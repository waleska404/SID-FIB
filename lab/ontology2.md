# Ontologías: SPARQL, JENA

###### tags: `SID-lab`

* [Introducción](#introducción)
* [Consultas](#consultas)
   * [Estructura](#estructura)
   * [Ejemplos](#ejemplos)
* [Modificadores Útiles](#modificadores-útiles)
* [DML](#dml)
* [JENA](#jena)
   * [Arquitectura](#arquitectura)
   * [Set up](#set-up)
   * [JenaTester](#jenatester)
   * [Cargar Ontología](#cargar-ontología)
   * [Niveles de Inferencia](#niveles-de-inferencia)
   * [Guardar ontología](#guardar-ontología)
   * [Listar instancias](#listar-instancias)
   * [Agrupar instancias por clase](#agrupar-instancias-por-clase)
   * [Consultar propiedades](#consultar-propiedades)
   * [Añadir elementos a la ontología](#añadir-elementos-a-la-ontología)
   * [Consultar con SPARQL](#consultar-con-sparql)
   * [Usar diferentes niveles de inferencia](#usar-diferentes-niveles-de-inferencia)
* [Referencias](#referencias)



---

## Introducción

* SPARQL Protocol and RDF Query Language.
* Lenguaje de consultas de facto para la web semántica.
* Funciona bajo RDF. Consultas basadas en tripletas.
* Permite consultas en datos estructurados y semiestructurados.
* Permite consultas sobre las estructuras de datos de forma natural.
* Permite joins sobre bases de conocimiento no homogéneas.
* Dispone de algunas extensiones.
    * GeoSPARQL
    * SPARUL
        * SPARQL con DML
            * INSERT
            * UPDATE
* Versión 1.0 de 2008.
    * Versión 1.1 de 2013.


---

## Consultas

### Estructura

* Prefijos: Permiten abreviar URIs que de otra forma serían muy largas (opcionales).
* Definición de modelos: Sobre qué modelos RDF hacemos la consulta.
* Resultado: Información que estamos obteniendo.
* Patrón de consulta: Cómo obtenemos dicha información.
* Modificadores de consulta: División, ordenado, etc.


```python
#prefix declarations
PREFIX foo:<http://example.com/resources/>
#dataset definition
FROM ...
#result
                 clause
SELECT
#query pattern
WHERE{
}
#query modifiers
ORDER BY ...
```


### Ejemplos

#### Ejemplo I

```
select distinct ?Concept where {[] a ?Concept} LIMIT 100

PREFIX dbpedia: <http://dbpedia.org/property/birthName>
PREFIX actor: <http://dbpedia.org/ontology/Actor>
SELECT *
WHERE {
    ?actor a <http://dbpedia.org/ontology/Actor>.
?actor <http://dbpedia.org/property/birthName> ?nombre

}LIMIT 50
```

* ?Variable
* . Al final de cada línea en el WHERE
* WHERE va entre corchetes, no paréntesis
* Uso de tripletas: Notad como saltamos entre nodos


#### Ejemplo II

```
PREFIX actor: <http://dbpedia.org/ontology/Actor>
SELECT ?nombreActor, ?nombrePeli
WHERE {
    ?actor a <http://dbpedia.org/ontology/Actor>.
?peli <http://dbpedia.org/ontology/starring> ?actor.
?actor <http://dbpedia.org/property/name> ?nombreActor.
?peli <http://xmlns.com/foaf/0.1/name> ?nombre Peli.
} LIMIT 50
```

```
PREFIX actor: <http://dbpedia.org/ontology/Actor>
SELECT ?nombreActor, ?nombre Peli
WHERE{
    ?actor a <http://dbpedia.org/ontology/Actor>.
?peli <http://dbpedia.org/ontology/starring> ?actor.
?actor <http://dbpedia.org/property/name> ?nombreActor.
?peli <http://xmlns.com/foaf/0.1/name> ?nombre Peli.
?actor <http://dbpedia.org/property/name> "Bruce Lee"@en.         
} LIMIT 50
```

```
PREFIX actor: <http://dbpedia.org/ontology/Actor>
SELECT ?nombreActor, ?nombre Peli
WHERE{
    ?actor a <http://dbpedia.org/ontology/Actor>.
?peli <http://dbpedia.org/ontology/starring> ?actor.
?actor <http://dbpedia.org/property/name> ?nombreActor.
?peli <http://xmlns.com/foaf/0.1/name> ?nombre Peli.
FILTER regex(?nombreActor,"^Bruce")
} LIMIT 50
```

---

## Modificadores Útiles

* `a (rdf:type)`
* `LIMIT`
* `ORDER BY`
    * `ORDER BY ?X DESC ?Y`
* `OFFSET`
* `DISTINCT`
* `CONSTRUCT` (Grafo RDF como resultado)
* `DESCRIBE` (Descripción de un grafo RDF), e.g.:
    `DESCRIBE <http://purl.uniprot.org/core/>`
* `FILTER`, `MINUS`
    * `SELECT * {?s ?p ?o FILTER NOT EXISTS {?s ?y ?z}}`
    * `SELECT * {?s ?p ?o FILTER REGEX(?s, STRING, "i")}`
        * `FILTER REGEX` funciona como `LIKE` en SQL
    * `SELECT * {?s ?p ?o MINUS {?x ?y ?z}}`
    * ``FILTER(LANG(?label) = "" ||
        LANGMATCHES(LANG(?label), "en"))``
* `BIND`
    * SELECT ?nombre ?precioFinal
        {?x precio ?precio . ?x descuento ?descuento.
        ?x nombre ?nombre .
        BIND (?precio * (1 - ?descuento) AS ?precioFinal)}
* `ASK` (boolean como resultado)
* `OPTIONAL` (Bases heterogeneas)
* `SameTerm` (?X, ?Y)
* Comentarios: `# Esto es un comentario`


---

## DML

* INSERT

```
INSERT{
 <http:// example/libro> titulo "Snowcrash";
                         Autor "Neal Stephenson";
                         Precio "Un huevo"} WHERE{}
```

* DELETE

```
DELETE{?x} WHERE {?xtitulo"SnowCrash"}
   PREFIX foaf: <http://xmlns.com/foaf/0.1/>
   WITH <http:// example/addresses>
   DELETE { ?person foaf:givenName 'Bill' }
   INSERT { ?person foaf:given Name 'William' }
   WHERE { ?person foaf:givenName' Bill' }
```

* UPDATE

```
INSERT DATA{
 <http:// example/libro> PrecioReal "Muy caro" }
DELETE DATA{
 <http:// example/libro> Precio Real "Muy caro" }
```

* Otras operaciones (según configuración del motor):
    * LOAD
    * COPY
    * MOVE
    * CLEAR


----

## JENA

### Arquitectura

![](images/ontology2/1.png)


### Set up

* Proyecto Apache Jena
    * RDF + OWL APIs
    * SPARQL Server + UI (Fuseki)
* Descargad las librerías de las APIs y el código de ejemplo:
    * https://dlcdn.apache.org/jena/binaries/apache-jena-4.4.0.zip
    * https://gitlab.fib.upc.edu/sergio.alvarez-apagao/materialsid/raw/master/jena/JenaTester.java
* Importad los siguientes .jar al CLASSPATH (JDK 11):
    * jena-core-4.4.0
    * jena-base-4.4.0
    * jena-arq-4.4.0
    * jena-iri-4.4.0
    * jena-shaded-guava-4.4.0
    * libthrift-0.15.0
    * slf4j-api-1.7.35
    * commons-lang3-3.12.0

### JenaTester

![](images/ontology2/2.png)

### Cargar Ontología

![](images/ontology2/3.png)


### Niveles de Inferencia

![](images/ontology2/4.png)
![](images/ontology2/5.png)

* La decisión dependerá de las necesidades.
    * TRANS_INF es mucho más rápido que RULE_INF
    * MICRO es mucho más rápido que MINI o DL
* Otra opción es usar un razonador externo (e.g. Pellet)
* Documentación
    * https://jena.apache.org/documentation/inference/index.html
    * https://jena.apache.org/documentation/ontology/

### Guardar ontología

![](images/ontology2/6.png)

### Listar instancias


![](images/ontology2/7.png)


```
Get all individuals
Ontology has individual:
   http://www.co-ode.org/ontologies/pizza/pizza.owl#England
   hasPizzaName=null
Ontology has individual:
   http://www.co-ode.org/ontologies/pizza/pizza.owl#France
   hasPizzaName=null
Ontology has individual:
   http://www.co-ode.org/ontologies/pizza/pizza.owl#America
   hasPizzaName=null
Ontology has individual:
   http://www.co-ode.org/ontologies/pizza/pizza.owl#Italy
   hasPizzaName=null
Ontology has individual:
   http://www.co-ode.org/ontologies/pizza/pizza.owl#Germany
   hasPizzaName=null
```

### Agrupar instancias por clase


![](images/ontology2/8.png)


```
Class:'http://www.co-ode.org/ontologies/pizza/pizza.owl#Country' has individuals:
    •http://www.co-ode.org/ontologies/pizza/pizza.owl#Italy
    •http://www.co-ode.org/ontologies/pizza/pizza.owl#Germany
    •http://www.co-ode.org/ontologies/pizza/pizza.owl#France
    •http://www.co-ode.org/ontologies/pizza/pizza.owl#England
    •http://www.co-ode.org/ontologies/pizza/pizza.owl#America
```

### Consultar propiedades

![](images/ontology2/9.png)


```
Name:hasBase
      •Domain :...#Pizza
      •Range :...#PizzaBase
      •Inverse :false
      •IsData :false
      •Is Functional :true
      •IsObject :true
      •IsSymetric :false
      •IsTransitive :false
```

### Añadir elementos a la ontología

![](images/ontology2/10.png)

### Consultar con SPARQL


![](images/ontology2/11.png)


```
Pizza=...#FourSeasonsInstance<->false
Pizza=...#FourSeasonsInstance<->true            
```


### Usar diferentes niveles de inferencia


![](images/ontology2/12.png)


```
FourSeasonsInstance classifies as RealItalianPizza ?: true
FourSeasonsInstance classifies as SpicyPizza ?: false
```

---

## Referencias 

* https://www.w3.org/TR/2013/REC-sparql11-query-20130321/
* https://www.w3.org/TR/2013/REC-sparql11-update-20130321/
* https://jena.apache.org/documentation/inference/
* https://jena.apache.org/documentation/ontology/
