# Ejercicios - Ontologías, Protégé y OWL

###### tags: `SID-lab`

[ToC]

---

## Ejercicio 1

1. Descargad la ontología (https://raw.githubusercontent.com/owlcs/pizza-ontology/master/pizza.owl) y cargarla en Pretégé.
2. Añadid algún comentario (Annotations).
    **PNG 1**
3. Cread una subclase de Thing (Entities).
    **PNG 2**
4. Cread un hermano y una subclase de esta clase.
5. Haced que la clase y su hermano sean disjuntas (Disjoint With). No hace falta hacerlo para las dos.
    **PNG 3**

---
    
## Ejercicio 2

Observad la diferencia entre `NamedPizza` y `RealItalianPizza`:
1. ¿Cuál es primitiva y cuál equivalente?
    `NamedPizza` es la primitiva y `RealItalianPizza` es la equivalente.
    **PNG 4**
    **PNG 5**
3. ¿Cuáles son las condiciones suficientes para que una pizza sea `RealItalianPizza`?
    Que sea una `Pizza` y que tenga como valor de `hasCountryOfOrigin`: `Italy`.
    **PNG 6**
5. ¿Qué condiciones añade a las suficientes?
    Que tenga `only ThinAndCrispyBase`.
    **PNG 7**
    
    
---

## Ejercicio 3

1. Arrancad el Reasoner incluído en Protégé. Se puede configurar para ampliar/acotar el ámbito de lógica.
2. Analizad inconsistencias:
    * Buscad las inconsistencias (en rojo).
    * ¿A qué se deben estas inconsistencias?
    * Usad el símbolo de interrogación para obtener explicaciones.
    **PNG 8**
    **PNG 9**
    **PNG 10**
    **PNG 11**
3. Analizad la clasificación del razonador.
    * Buscad las inferencias de clasificación (en amarillo).
    * Usad el símbolo de interrogación para obtener explicaciones.
    Por ejemplo:
    **PNG 12**
    **PNG 13**
    **PNG 14**
4. Parad el Reasoner.
    **PNG 15**

---

## Ejercicio 4

1. Cread una ObjectProperty para expresar en qué país se vende.
    **PNG 16**
    * Asignad dominio y rango
    **PNG 17**
    **PNG 18**
2. Cread una subpropiedad de `hasIngredient` para poder representar el relleno del borde.
    **PNG 19**
    * Asignad dominio y rango.
    * Asignad alguna restricción, como por ejemplo `disjoint with` o `inverse of`.
    **PNG 20**
3. Cread una DataProperty para poder representar el precio.
    **PNG 21**
    * Asignad dominio y rango.
    **PNG 22**
    **PNG 23**
    
    
---

## Ejercicio 5

* Cread una instancia de DeepPanBase (Individuals).
    **PNG 24**
    **PNG 25**
* Cread una instancia de Pizza con las siguientes propiedades:
    * Tiene como país de origen Italia.
    **PNG 26**
    * Tiene como base la instancia de DeepPanBase que habéis creado.
    **PNG 27**
    **PNG 28**
* En el menú, arrancad el Reasoner
    * ¿Es inconsistente? ¿Por qué?
    **PNG 29**
    **PNG 30**
* Borrad estas instancias y volved a sincronizar el Reasoner.

---

## Ejercicio 6


* Cread un topping TurtleTopping.
    **PNG 31**
* Cread una Pizza llamada SuperMarioPizza con condiciones necesarias y suficientes: tener como ingredientes champiñones y tortugas.
    **PNG 32**
    **PNG 33**
* Cread una instancia de una pizza de tipo Pizza con ingredientes instancias de champiñones y tortugas.
    **PNG 34**
* Sincronizad el Razonador y observad cómo se clasifica.
    **PNG 35**
* Cambiad SuperMarioPizza para que las condiciones sean sólo necesarias y observad la diferencia tras sincronizar.
    **PNG 36**
    **PNG 37**
    
---

## Ejercicio 7

* Cread las siguientes pizzas:
    * Pizza con marisco: contiene como mínimo marisco.
    **PNG 38**
    * Pizza de marisco: todos los ingredientes son de marisco.
    **PNG 39**
    * Pizza ecléctica: mínimo 10 ingredientes.
    **PNG 40**
    * Pizza de oferta: máximo 2 ingredientes.
    **PNG 41**
    * Pizza binaria: exactamente 2 ingredientes.
    **PNG 42**
    * Pizza triqueso: exactamente 3 ingredientes, todos de queso.
    **PNG 43**
    * Pizza escandinava:
        * Tendréis que editar en texto libre (Class Expression Editor) y también editar la clase Country.
        * Utilizad or y value (tenéis ejemplos en American y en la guía).
    **PNG 44**
    * Pizza aburrida especial: pizzas que no sean InterestingPizza, pero que estén en la unión entre las MeatyPizza y las CheesyPizza.
    **PNG 45**
    

---

## Ejercicio 8

1. Cread una propiedad funcional que asigne un creador a una NamedPizza (tendréis que crear clases).
    * Asignad dos creadores a una instancia de NamedPizza.
    **PNG 46**
    * Sincronizad el Razonador.
    * Qué inferencia ha hecho?
    Ha determinado que las dos creadoras son el mismo individual.
    **PNG 47**
    **PNG 48**
2. Identificad los creadores como Different Individuals y resincronizad.
    **PNG 49**
3. Cread una propiedad transitiva que permita representar que la creación de una NamedPizza está influenciada por otra.
    **PNG 50**
4. Cread una propiedad simétrica que permita expresar que dos ingredientes combinan bien.
    **PNG 51**
5. Observad las características disponibles en las data properties. ¿Tiene sentido?
    Si. Solo está disponible la `Funcional`.