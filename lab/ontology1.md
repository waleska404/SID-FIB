# Ontologías, Protégé y OWL

###### tags: `SID-lab`

[ToC]

---

## Teoría básica sobre Ontologías

### Filosofía (Aristóteles y Platón)

Filosóficamente: Parte de la metafísica que estudia lo que hay:
* Lo que existe. Entidades o conjuntos de entidades.
* Formas en que se relacionan las entidades que existen.

### Informática

* Esquema conceptual (detallado) de un domino (o varios).
* Facilita la comunicación (intercambio de información) entre sistemas heterogéneos.
* Representación del conocimiento. Estructura que contiene todas las entidades y relaciones relevantes para el dominio tratado.
* Cyc (Ontología con conocimiento genérico).
* Uso en Inteligencia Artificial:
    * Razonamiento.
    * Clasificación.

### Base tecnológica

* DAML
    * Fuertemente asociado a WebServices.
    * DARPA.
* OIL
    * Comisión Europea.
    * Primer lenguaje de intercambio de Ontologías.
    * Anticuado y poco expresivo.
* RDF
    * Resource description framework.
    * Esquema general de representación de información.
    * Sin semántica asociada.
* **OWL**
    * Inspirado en DAML y OIL.
    * Construido sobre RDF + XML.

### RDF Schema
https://www.w3.org/TR/rdf-schema/
* Classes
    * `rdfs:Resource`
    * `rdfs:Class`
    * `rdfs:Literal`
    * `rdfs:Datatype`
    * `rdf:langString`
    * `rdf:HTML`
    * `rdf:XMLLiteral`
    * `rdf:Property`
* Properties
    * `rdfs:range`
    * `rdfs:domain`
    * `rdf:type`
    * `rdfs:subClassOf`
    * `rdfs:subPropertyOf`
    * `rdfs:label`
    * `rdfs:comment`

---

## Ontology Web Language (OWL)

* OWL-FULL
    * Sin restricciones.
    * Permite bucles en las relaciones.
    * Algunas sentencias pueden llevar tiempo infinito en resolverse.
* OWL-DL
    * Termino medio.
    * Basado en lógica descriptiva.
    * Contiene algunas restricciones.
* OWL-LITE
    * Básico.
    * Taxonomía con restricciones simples.

![](https://i.imgur.com/iZabIdA.png)


### OWL Full

* `owl:Class` = `rdfs:Class`
    * Todos los documentos RDF son documentos OWL-FULL.
* `owl:Thing` = `rdfs:Resource`
* `owl:ObjectProperty` = `rdf:Property`
    * `owl:DatatypeProperty` hereda de `owl:ObjectProperty`.
* Un recurso puede ser a la vez clase e instancia.
    * Boeing-747 is an instance of the class AirplaneType.
    * airplane1 is an instance of the class Boeing-747.
* Permite el uso de todas las restricciones definidas en OWL.
* Sin restricciones sobre los axiomas (pueden ser inconsistentes).

![](https://i.imgur.com/kFImHy9.png)


### OWL DL

* Permite todos los tipos de restricciones, con limitaciones.
    * Restricciones numéricas no soportadas en propiedades transitivas.
    * `owl:DatatypeProperty` no hereda de `owl:ObjectProperty`.
        * Propiedades como `inverseOf`, `SimmetricProperty` o `TransitiveProperty` no se pueden aplicar a `DatatypeProperties`.
    * Restricciones en las anotaciones (annotation property).
        * Sólo soporta datos, literales, URI o Instancias.
        * Una annotation property no puede tener sub-propiedades.
* Los axiomas definidos han de ser jerárquicos, correctos y consistentes (e.g. no depender de clases no declaradas).
    * Los axiomas sobre igualdad o diferencia han de referirse a las instancias (individuals).

### OWL Lite

* Restricciones de cardinalidad 0..1.
* No permite algunas restricciones importantes como `disjointWith`.
* Casi tan complejo como OWL-DL de modo que apenas se usa.

---

## Ciclo de desarrollo de una Ontología

![](https://i.imgur.com/rX4qgzO.png)

**1. Determine Scope**
* Cual es el dominio que intentamos cubrir con la Ontología.
    * Problema de la granularidad.
    * Problema de la omnisciencia.
* Para que vamos a usar la Ontología.
* Identificar las Competency Questions: Para qué tipos de preguntas debe darnos respuesta la información que contiene la Ontología.
* Las decisiones no son finales, pueden cambiar durante el ciclo de desarrollo de la Ontología.

**2. Consider Reuse**
* ¿Por qué?
    * Eficiencia, menor coste de desarrollo.
    * Integración directa con sistemas que usen esa Ontología.
    * Uso de Ontologías que han sido validadas en casos de uso prácticos (aplicaciones).

**3. Enumerate Terms**
* Cuáles son los términos sobre los que vamos a hablar.
* Cuáles son las propiedades de esos términos.
* Qué queremos decir sobre esos términos.
* Primer paso: No organizar los términos, hacer una lista con lo que queremos incluir en la Ontología.

**4. Define Classes**
* Definir las clases y la taxonomía.
    * Una clase es un concepto del dominio, no un objeto.
        * ¡No sólo entidades, pueden ser propiedades!
    * Una clase es un conjunto de elementos con propiedades similares.
        * ¿Y qué es cada elemento entonces?
    * Top-Down: Definir primero los conceptos más generales, y luego especializar.
    * Bottom-up: Definir los conceptos más específicos y luego agruparlos en clases más generales.
    * Combinación: Definir los conceptos más importantes y luego generalizarlos y especificarlos en paralelo.
        * Útil si aplicamos otra de las dos técnicas y nos quedamos atascados.
    * Clases disjuntas: Una instancia no puede pertenecer a ambas clases a la vez.
* La taxonomía es la jerarquía de clases.
    * ¿Cuándo agrupamos dos clases en la misma superclase?
* **Tipos de clases:**
    * Primitiva: Necessary conditions.
        * Si algo reúne las condiciones no es necesariamente obligatorio que sea un miembro de la clase. ![](https://i.imgur.com/pthpE6G.png)
        * PERO: Un elemento escogido al azar que sabemos que es miembro de la clase, sabemos que reúne las condiciones.
        * ¿Qué ocurre con un elemento escogido al azar que sabemos que reúne las condiciones? Es posible que pertenezca a la clase pero también es posible que no.
    * Equivalente: Necessary conditions and sufficient conditions.
        * Si algo reúne las condiciones es suficiente para decir que es un miembro de la clase.
        * Un elemento escogido al azar que sabemos que es miembro de la clase, sabemos que reúne las condiciones.
        * ¿Qué ocurre con un elemento escogido al azar que sabemos que reúne las condiciones? Sabemos con certeza que pertenece a la clase. ![](https://i.imgur.com/jkknzZo.png)

**5. Define Properties**
* Asociadas a la clases (Dominio-Rango):
    * Rango no es una clase: `Data Properties`.
    * Rango es una clase: Relaciones a otras instancias de la clase, `Object Properties`.


**6. Define Constraints**
* Las restricciones definen el conjunto de valores posibles para una propiedad.
* Las restricciones más comunes son:
    * Dominio
    * Rango
* No son restricciones a comprobar, son axiomas.

**7. Create Instances**
* Crear instancias de las clases.
    * La clase se convierte en un tipo directo de la instancia.
    * Las superclases del tipo directo son tipos de la instancias.
* Asignar valores a las propiedades.
    * Los valores asignados deben cumplir las restricciones impuestas-
    * Se pueden usar razonadores para comprobar que las restricciones se cumplan.

### Ejemplo y Ejercicios: PizzaOntology


EJERCICIO 1
1. Descargad la ontología (https://raw.githubusercontent.com/owlcs/pizza-ontology/master/pizza.owl) y cargarla en Pretégé.
2. Añadid algún comentario (Annotations).
![](https://i.imgur.com/iO2DggP.png)
3. Cread una subclase de Thing (Entities)
![](https://i.imgur.com/NoDgR2M.png)
4. Cread un hermano y una subclase de esta clase.
![](https://i.imgur.com/vU5H6rF.png)
5. Haced que la clase y su hermano sean disjuntas (Disjoint With). No hace falta hacerlo para las dos.
![](https://i.imgur.com/4nWHgL7.png)


EJERCICIO 2

Observad la diferencia entre `NamedPizza` y `RealItalianPizza`:
1. ¿Cuál es primitiva y cuál equivalente?
    `NamedPizza` es la primitiva y `RealItalianPizza` es la equivalente.
    ![](https://i.imgur.com/w09N5fA.png)
    ![](https://i.imgur.com/Y57m0s1.png)
3. ¿Cuáles son las condiciones suficientes para que una pizza sea `RealItalianPizza`?
    Que sea una `Pizza` y que tenga como valor de `hasCountryOfOrigin`: `Italy`.
    ![](https://i.imgur.com/2r1oQen.png)
5. ¿Qué condiciones añade a las suficientes?
    Que tenga `only ThinAndCrispyBase`.
    ![](https://i.imgur.com/NnWXr9f.png)


EJERICICO 3

1. Arrancad el Reasoner incluído en Protégé. Se puede configurar para ampliar/acotar el ámbito de lógica.
2. Analizad inconsistencias:
    * Buscad las inconsistencias (en rojo).
    * ¿A qué se deben estas inconsistencias?
    * Usad el símbolo de interrogación para obtener explicaciones.
    ![](https://i.imgur.com/toG2dwh.png)
    ![](https://i.imgur.com/RRC5ycP.png)
    ![](https://i.imgur.com/trjzAIS.png)
    ![](https://i.imgur.com/vt3DHOW.png)
3. Analizad la clasificación del razonador.
    * Buscad las inferencias de clasificación (en amarillo).
    * Usad el símbolo de interrogación para obtener explicaciones.
    Por ejemplo:
    ![](https://i.imgur.com/vog1OWo.png)
    ![](https://i.imgur.com/tub17Kf.png)
    ![](https://i.imgur.com/DFRasWN.png)
4. Parad el Reasoner.
![](https://i.imgur.com/SVBh8UG.png)

EJERICCIO 4

1. Cread una ObjectProperty para expresar en qué país se vende.
    ![](https://i.imgur.com/8ZYl9zU.png)
    * Asignad dominio y rango
    ![](https://i.imgur.com/6LDO4JS.png)
    ![](https://i.imgur.com/qMWtCnz.png)
2. Cread una subpropiedad de `hasIngredient` para poder representar el relleno del borde.
    ![](https://i.imgur.com/P96sArR.png)
    * Asignad dominio y rango.
    * Asignad alguna restricción, como por ejemplo `disjoint with` o `inverse of`.
    ![](https://i.imgur.com/R6FRg8P.png)
3. Cread una DataProperty para poder representar el precio.
    ![](https://i.imgur.com/9VNXIov.png)
    * Asignad dominio y rango.
    ![](https://i.imgur.com/bj4lfrk.png)
    ![](https://i.imgur.com/sW8Dhk1.png)


EJERCICIO 5

* Cread una instancia de DeepPanBase (Individuals).
    ![](https://i.imgur.com/ICpolfc.png)
    ![](https://i.imgur.com/iOWlwfh.png)
* Cread una instancia de Pizza con las siguientes propiedades:
    * Tiene como país de origen Italia.
    ![](https://i.imgur.com/CxjmQPV.png)
    * Tiene como base la instancia de DeepPanBase que habéis creado.
    ![](https://i.imgur.com/bBLPnB7.png)
    ![](https://i.imgur.com/CuGmgUF.png)
* En el menú, arrancad el Reasoner
    * ¿Es inconsistente? ¿Por qué?
    ![](https://i.imgur.com/q7K3KEH.png)
    ![](https://i.imgur.com/nQvPyXY.png)
* Borrad estas instancias y volved a sincronizar el Reasoner.




EJERCICIO 6

* Cread un topping TurtleTopping.
    ![](https://i.imgur.com/g64NSIV.png)
* Cread una Pizza llamada SuperMarioPizza con condiciones necesarias y suficientes: tener como ingredientes champiñones y tortugas.
    ![](https://i.imgur.com/8ErBBnd.png)
    ![](https://i.imgur.com/WJhFaEF.png)
* Cread una instancia de una pizza de tipo Pizza con ingredientes instancias de champiñones y tortugas.
    ![](https://i.imgur.com/3MFaLT1.png)
* Sincronizad el Razonador y observad cómo se clasifica.
    ![](https://i.imgur.com/6pOvyFH.png)
* Cambiad SuperMarioPizza para que las condiciones sean sólo necesarias y observad la diferencia tras sincronizar.
    ![](https://i.imgur.com/08LCoH7.png)
    ![](https://i.imgur.com/oIlHcAP.png)


---

## Restricciones

* Algunas restricciones están disponibles en el editor de Protégé:
    ![](https://i.imgur.com/ynakpQZ.png)
* Guía para editar en texto libre: http://protegeproject.github.io/protege/class-expressionsyntax/

### Axiomas de Clase

* Enumeraciones de individuos: `oneOf`.
    * Permite describir una clase por sus posibles instancias.
* Clases excluyentes entre si: `disjointWith`.
    * Una instancia no puede pertenecer a las dos clases a la vez.
* Clases equivalentes entre si: `sameClassAs`.
    * No confundir con `equivalentClass`.
    * Todas las instancias de una clase han de ser instancias de la otra clase.
    * No todos los razonadores realizan la inferencia (ineficiente).
    * En cualquier caso es útil para enlazar ontologías.


### Quantifier Restrictions

* Existencial: `some`.
    * Una pizza picante es una pizza que contiene al menos un ingrediente picante.
* Universal: `only`.
    * Una pizza vegetariana es una pizza donde todos los ingredientes son de origen no animal.

### Cardinality Restrictions

* Mínimo número de relaciones: `minCardinality`.
* Máximo número de relaciones: `maxCardinality`.
* Número exacto de relaciones: `cardinality`.
* Restricciones cualificadas: Limitan el rango de la relación.

### Restricciones por Valor

* `hasValue` restrictions:
    * Equivalente a enumeraciones de instancias.
    * Usa el símbolo: ![](https://i.imgur.com/zGuzX0c.png)
    ![](https://i.imgur.com/GbYRltg.png)

### Operaciones de Conjuntos

* Intersección de dos clases:
    * `intersectionOf`
    * En Protégé: `classA and ClassB`
* Unión de dos clases:
    * `unionOf`
    * En Protégé: `classA or ClassB`
* Complemento de una clase (todas las instancias que no pertenecen a esa clase):
    * `complementOf`
    * En Protégé: `not classA`

### Ejercicio

* Cread las siguientes pizzas:
    * Pizza con marisco: contiene como mínimo marisco.
    ![](https://i.imgur.com/cLDTWyK.png)
    * Pizza de marisco: todos los ingredientes son de marisco.
    ![](https://i.imgur.com/yQyBa7z.png)
    * Pizza ecléctica: mínimo 10 ingredientes.
    ![](https://i.imgur.com/cIrgLPY.png)
    * Pizza de oferta: máximo 2 ingredientes.
    ![](https://i.imgur.com/qVOBBq2.png)
    * Pizza binaria: exactamente 2 ingredientes.
    ![](https://i.imgur.com/5Qx7m3s.png)
    * Pizza triqueso: exactamente 3 ingredientes, todos de queso.
    ![](https://i.imgur.com/hoHQXsE.png)
    * Pizza escandinava:
        * Tendréis que editar en texto libre (Class Expression Editor) y también editar la clase Country.
        * Utilizad or y value (tenéis ejemplos en American y en la guía).
    ![](https://i.imgur.com/XpshZM0.png)
    * Pizza aburrida especial: pizzas que no sean InterestingPizza, pero que estén en la unión entre las MeatyPizza y las CheesyPizza.
    ![](https://i.imgur.com/IF4KGIu.png)

---

## Propiedades

* Propiedades y subpropiedades: ¿Cuándo agrupamos propiedades en subpropiedades?
* Domino y rango de la propiedad. ¡Recordad que son tratadas como axiomas!
* **Propiedad Inversa**
    * Del tipo `hasComponent` vs `isComponentOf`.
    * Donde el dominio y el rango, se intercambian.
* **Propiedad Funcional**
    * Cuando A y B están relacionados mediante una propiedad funcional sólo una instancia de B puede estar relacionada con A. ¿Qué ocurre si más de una instancia de B está relacionada con A?
    ![](https://i.imgur.com/fzaTIXW.png)
* **Propiedad Funcional Inversa** (e.g. número de serie).
* **Propiedad Transitiva**
    * Si una instancia de A se relaciona con una de B y una de B con C, la instancia de A se relaciona con la de C.
* **Propiedad Simétrica**
    * Si una instancia de A se relaciona con una de B, la de B se relaciona con la de A.
* **Propiedad Asimétrica (antisimétrica)**
    * Si una instancia de A se relaciona con una de B, la de B no se puede relacionar con la de A.
* **Propiedad Reflexiva**
    * Si P es reflexiva y una instancia A tiene P, P se aplica a la instancia de A.
* **Propiedad Irreflexiva**
    * Si P es reflexiva y una instancia A tiene P, P no se puede aplicar a la instancia de A.


### Ejercicio

1. Cread una propiedad funcional que asigne un creador a una NamedPizza (tendréis que crear clases).
    * Asignad dos creadores a una instancia de NamedPizza.
    ![](https://i.imgur.com/Kc3WqJF.png)
    * Sincronizad el Razonador.
    * Qué inferencia ha hecho?
    Ha determinado que las dos creadoras son el mismo individual.
    ![](https://i.imgur.com/WsRz1MS.png)
    ![](https://i.imgur.com/VFT3lAU.png)
2. Identificad los creadores como Different Individuals y resincronizad.
    ![](https://i.imgur.com/Ca1gcoN.png)
3. Cread una propiedad transitiva que permita representar que la creación de una NamedPizza está influenciada por otra.
    ![](https://i.imgur.com/ZizN2ab.png)
4. Cread una propiedad simétrica que permita expresar que dos ingredientes combinan bien.
    ![](https://i.imgur.com/lcaLeaA.png)
5. Observad las características disponibles en las data properties. ¿Tiene sentido?
    Si. Solo está disponible la `Funcional`.

---
## Referencias 

* Cyc
    * http://www.cyc.com/
    * http://www.opencyc.org/
* DAML
    * http://www.daml.org/
* OIL
    * http://www.cs.vu.nl/~frankh/postscript/IEEE-IS01.pdf
* RDF
    * http://www.xml.com/pub/a/2001/01/24/rdf.html
* OWL
    * http://owl.cs.manchester.ac.uk/tutorials/protegeowltutoria
* Protégé
    * http://protege.stanford.edu
* Ontologia de pizzas
    * www.co-ode.org/ontologies/pizza/