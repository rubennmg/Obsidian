## Funciones de pérdida
Miden la diferencia entre lo que se predice y lo que realmente es.

## Algoritmos 
##### Zero R
Aprende reglas que tiene 0 condiciones
![[Pasted image 20230131141405.png]]
siempre devuelve la moda, es decir, el valor que más se repite, (0 condiciones)


##### OneR
Algortimos que incluyen UNA condición
En el ejemplo anterior, se concluye sí o no en función de una pregunta
![[Pasted image 20230131141806.png]]


##### Instance based learning
Vecino más próximo

El problema de este algorimo es calcular la distancia (diferencia entre dos valores)
Los resultados se suelen normalizar
Si algún atributo es *nominal* (en el caso de los lirios, el color) ¿cómo se calcula la distancia entre colores? Se debe de hacer algún tipo de aproximación


##### k-NN
Preguntar a más de un vecino próximo. Si hay dos clases conviene que el número de vecinos sea impar, para que no haya empates


## Función de pérdida (2022)
![[Pasted image 20230131143211.png]]
Problema de optimización (calcular máximos y mínimos, en este caso mínimos)
Buscar parámetros (y sus pesos) que hagan que la pérdida sea mínima
D -> conjunto de datos (pares x e y) (lo llama también: ejemplo de entrenamiento)


## Árboles de decisión
Se da un caso para que se clasifique, entonces el árbol pregunta ¿cuál es el valor del atributo A?
	este puede ser a1, a2 o a3. Si es a3 ->SI, si es a2 pregunta por B, que puede ser b1 o b2 ...
	![[Pasted image 20230131144354.png]]
###### Estructura
Nodos 
Hojas
Se empieza por la raíz

##### Construcción de árboles de decisión
Funciones para valorar proporciones de sí y no en cada atributo


## C4.5 (v 1993)
p_j -> probabilidad de que se dé una determinada clase
![[Pasted image 20230131145112.png]]





# Tema 2. Aprendizaje automático 3

![[Pasted image 20230202131136.png]]
Principio de evaluación
	- clave para que todo funcione
	- debe de hacerse sobre principios de datos nuevos
	- capacidad de generalización
![[Pasted image 20230202131330.png]]
Errores/fallos en evaluación
	- número de clasificaciones correctas
	- cantidad de aciertos
	- estimación del error numérico

Interesa tener un conjunto de test que sea independiente del conjunto de entrenamiento


El algoritmo del vecino más próximo tiene como parámetro el número de vecinos a los que se pregunta.
No es correcto utilizar el conjunto de test para ver cual es el mejor parámetro, porque el conjunto de test es una metáfora de datos futuros. El conjunto de entrenamiento también puede dividirse en entrenamiento y validación.


El conjunto de test se utiliza para estimar el error en casos no vistos. 


Si el conjunto de datos es limitado:
	- separar en entrenamiento y test
	- el problema es que las muestras que se generan en la separación tienen que ser representativas. 
	- usar versiones estratificadas (muestras estratificadas) 
	- estratificado: que representen la misma proporción tanto en entrenamiento como en test
	- ![[Pasted image 20230202133007.png]]
		mismas proporciones respecto al conjunto de datos inicial
	Puede darse el caso de que los datos, aún así, no estén bien distribuidos, para ello se ha de repetir (repeated holdout method)


**Validación cruzada (cross validation)**
Método que trata de solventar los problemas anteirores (aprovechar todos los ejemplos, distribución correcta)

Consiste en:
![[Pasted image 20230202133509.png]]
	- coger todos los ejemplso disponibles
	- se dividen en varias partes (n)
	- se selecciona una de las partes (todo estratificado)
	- las 9 restantes se cogen como conjunto de entrenamiento
	- se aprende algo y se evalúa en la parte restante
	- se selecicona otro trozo de nuevo
	- se aprende con los 9 restantes
	- así con todos los trozos
	- se aprenden tantas veces como partes haya
	- cada elemento sirve 9 veces para entrenamiento y 1 para test
	- los resultados (media) se guardan para hacer estimaciones de acierto/error

![[Pasted image 20230202133648.png]]
	- otro método
	- se entrega el clasificador y el número (estimación, la medida media de los aciertos de la evaluación)
	- **inconvenientes**
		  - tarda más (depende de lo que tarde el algoritmo ML)

en el libro aparece esto también (validación cruzada y más), importante mirarlo, lo ha dicho en clase

**Caso extremo de validación cruzada -> con tantos trozos como ejemplos haya (Leave-One-Out cross-validation)**
- Lleva más tiempo
- Es _aparentamente_ mejor, ya que normalmente no lo es y no sale rentable hacerlo (más largo, más costoso y no siempre fiable)



estudiar método SVM (importante pero no lo ha mirado)



