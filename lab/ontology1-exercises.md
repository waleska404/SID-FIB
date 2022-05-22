# Ejercicios - Ontologías, Protégé y OWL

###### tags: `SID-lab`

[ToC]

---

## Ejercicio 1

1. Descargad la ontología (https://raw.githubusercontent.com/owlcs/pizza-ontology/master/pizza.owl) y cargarla en Pretégé.
2. Añadid algún comentario (Annotations).
    ![](images/ontology1/exercises/1.png)
3. Cread una subclase de Thing (Entities).
    ![](images/ontology1/exercises/2.png)
4. Cread un hermano y una subclase de esta clase.
5. Haced que la clase y su hermano sean disjuntas (Disjoint With). No hace falta hacerlo para las dos.
    ![](images/ontology1/exercises/3.png)

---
    
## Ejercicio 2

Observad la diferencia entre `NamedPizza` y `RealItalianPizza`:
1. ¿Cuál es primitiva y cuál equivalente?
    `NamedPizza` es la primitiva y `RealItalianPizza` es la equivalente.
    ![](images/ontology1/exercises/4.png)
    ![](images/ontology1/exercises/5.png)
3. ¿Cuáles son las condiciones suficientes para que una pizza sea `RealItalianPizza`?
    Que sea una `Pizza` y que tenga como valor de `hasCountryOfOrigin`: `Italy`.
    
    ![](images/ontology1/exercises/6.png)
5. ¿Qué condiciones añade a las suficientes?
    Que tenga `only ThinAndCrispyBase`.
    ![](images/ontology1/exercises/7.png)
    
    
---

## Ejercicio 3

1. Arrancad el Reasoner incluído en Protégé. Se puede configurar para ampliar/acotar el ámbito de lógica.
2. Analizad inconsistencias:
    * Buscad las inconsistencias (en rojo).
    * ¿A qué se deben estas inconsistencias?
    * Usad el símbolo de interrogación para obtener explicaciones.
    
    ![](images/ontology1/exercises/8.png)
    ![](images/ontology1/exercises/9.png)
    ![](images/ontology1/exercises/10.png)
    ![](images/ontology1/exercises/11.png)
3. Analizad la clasificación del razonador.
    * Buscad las inferencias de clasificación (en amarillo).
    * Usad el símbolo de interrogación para obtener explicaciones.
    Por ejemplo:
    ![](images/ontology1/exercises/12.png)
    ![](images/ontology1/exercises/13.png)
    ![](images/ontology1/exercises/14.png)
4. Parad el Reasoner.

    ![](images/ontology1/exercises/15.png)

---

## Ejercicio 4

1. Cread una ObjectProperty para expresar en qué país se vende.

    ![](images/ontology1/exercises/16.png)
    * Asignad dominio y rango
    ![](images/ontology1/exercises/17.png)
    ![](images/ontology1/exercises/18.png)
2. Cread una subpropiedad de `hasIngredient` para poder representar el relleno del borde.
    ![](images/ontology1/exercises/19.png)
    * Asignad dominio y rango.
    * Asignad alguna restricción, como por ejemplo `disjoint with` o `inverse of`.
    
    ![](images/ontology1/exercises/20.png)
3. Cread una DataProperty para poder representar el precio.

    ![](images/ontology1/exercises/21.png)
    * Asignad dominio y rango.
    ![](images/ontology1/exercises/22.png)
    ![](images/ontology1/exercises/23.png)
    
    
---

## Ejercicio 5

* Cread una instancia de DeepPanBase (Individuals).

    ![](images/ontology1/exercises/24.png)
    ![](images/ontology1/exercises/25.png)
* Cread una instancia de Pizza con las siguientes propiedades:
    * Tiene como país de origen Italia.
    ![](images/ontology1/exercises/26.png)
    * Tiene como base la instancia de DeepPanBase que habéis creado.
   
    ![](images/ontology1/exercises/27.png)
    ![](images/ontology1/exercises/28.png)
* En el menú, arrancad el Reasoner
    * ¿Es inconsistente? ¿Por qué?

    ![](images/ontology1/exercises/29.png)
    ![](images/ontology1/exercises/30.png)
* Borrad estas instancias y volved a sincronizar el Reasoner.

---

## Ejercicio 6


* Cread un topping TurtleTopping.

    ![](images/ontology1/exercises/31.png)
* Cread una Pizza llamada SuperMarioPizza con condiciones necesarias y suficientes: tener como ingredientes champiñones y tortugas.
    ![](images/ontology1/exercises/32.png)
    ![](images/ontology1/exercises/33.png)
* Cread una instancia de una pizza de tipo Pizza con ingredientes instancias de champiñones y tortugas.
    ![](images/ontology1/exercises/34.png)
* Sincronizad el Razonador y observad cómo se clasifica.
    ![](images/ontology1/exercises/35.png)
* Cambiad SuperMarioPizza para que las condiciones sean sólo necesarias y observad la diferencia tras sincronizar.
    ![](images/ontology1/exercises/36.png)
    ![](images/ontology1/exercises/37.png)
    
---

## Ejercicio 7

* Cread las siguientes pizzas:
    * Pizza con marisco: contiene como mínimo marisco.
    
    ![](images/ontology1/exercises/38.png)
    * Pizza de marisco: todos los ingredientes son de marisco.
   
    ![](images/ontology1/exercises/39.png)
    * Pizza ecléctica: mínimo 10 ingredientes.
   
    ![](images/ontology1/exercises/40.png)
    * Pizza de oferta: máximo 2 ingredientes.
   
    ![](images/ontology1/exercises/41.png)
    * Pizza binaria: exactamente 2 ingredientes.
   
    ![](images/ontology1/exercises/42.png)
    * Pizza triqueso: exactamente 3 ingredientes, todos de queso.
    
    ![](images/ontology1/exercises/43.png)
    * Pizza escandinava:
        * Tendréis que editar en texto libre (Class Expression Editor) y también editar la clase Country.
        * Utilizad or y value (tenéis ejemplos en American y en la guía).
     
    ![](images/ontology1/exercises/44.png)
    * Pizza aburrida especial: pizzas que no sean InterestingPizza, pero que estén en la unión entre las MeatyPizza y las CheesyPizza.
    ![](images/ontology1/exercises/45.png)
    

---

## Ejercicio 8

1. Cread una propiedad funcional que asigne un creador a una NamedPizza (tendréis que crear clases).
    * Asignad dos creadores a una instancia de NamedPizza.
    ![](images/ontology1/exercises/46.png)
    * Sincronizad el Razonador.
    * Qué inferencia ha hecho?
    Ha determinado que las dos creadoras son el mismo individual.
    ![](images/ontology1/exercises/47.png)
    ![](images/ontology1/exercises/48.png)
2. Identificad los creadores como Different Individuals y resincronizad.

    ![](images/ontology1/exercises/49.png)
3. Cread una propiedad transitiva que permita representar que la creación de una NamedPizza está influenciada por otra.
    ![](images/ontology1/exercises/50.png)
4. Cread una propiedad simétrica que permita expresar que dos ingredientes combinan bien.
    ![](images/ontology1/exercises/51.png)
5. Observad las características disponibles en las data properties. ¿Tiene sentido?
    Si. Solo está disponible la `Funcional`.
