<center> <h1> Mecánica Homemade: <br>Tiempo de Creación de Objetos </h1></center>

## ¿Qué es?
Ésta mecánica cumple el propósito de poder crear objetos con algún NPC que esté habilitado para esto. Principalmente indica cuanto tiempo se demorará el NPC en conseguir un resultado, el cual tiene una posibilidad de fallar.

Intenta tener en cuenta los siguientes aspectos:
+ Complejidad del objeto creado
+ Tamaño del objeto creado
+ Habilidad para crear cosas
+ Proficiencia con las herramientas
+ Éxito en el resultado
## ¿Cómo funciona?
### 1. Elegir el objeto a crear
Lo primero es seleccionar el objeto que se busca crear. Esto puede ser un objeto que ya exista en DND o puede ser algo externo. En el caso de que ya exista, lo recomendable será tomar en cuenta sus estadísticas. El objeto determina que tan complejo es y que tamaño tendrá 
### 2. Complejidad
Que tan complejo es un objeto determina el tipo de dado que se usa para definir cuánto tiempo se tarda en crearlo. (Mínimo 1)

| Complejidad          | Dado       | Factor |
| -------------------- | ---------- | ------ |
| Trivial              | d1         | 0.05   |
| Sencillo             | d4         | 0.1    |
| Simple               | d6         | 0.2    |
| Comprensible         | d8         | 0.35   |
| Confuso              | d10        | 0.55   |
| Complejo             | d12        | 0.8    |
| Técnico              | d20        | 1      |
| Sumamente<br>Técnico | Porcentual | 2      |
El dado indica cuantos días demorará en crearse el objeto. Aunque queda a merced del DM si indican horas, días, semanas, meses o años ==**antes**== de lanzar los dados.

> [!star] Habilidad Superior
> Si el personaje es particularmente hábil creando el objeto o ya ha creado varias veces este objeto, entonces es capaz de bajar en una categoría de complejidad (Mínimo es "Trivial"). Si es extremadamente hábil en el proceso de creación podrá bajar 2 categorías como máximo.
> 
> Recomendación: no dar a un personaje habilidad superior con una gran cantidad de objetos. Si un personaje tendrá habilidad superior con varios objetos, tener en consideración la complejidad de estos; No es lo mismo saber hacer 10 objetos "Triviales" que 10 Objetos "Sumamente Técnicos".
> 
> Queda a merced del DM decidir cuando un NPC tiene habilidad superior con un objeto.

^083e43
> [!sparkles] Objetos Mágicos
> Un objeto mágico va a tener una complejidad mayor que su equivalente no mágico, y dependiendo de la magia que se le imbuye al objeto, este puede ser entre 1 a 3 categorías superiores.
### 3. Tamaño
El tamaño de el objeto indica cuantos dados se utilizan para determinar la cantidad de días. Los tamaños pueden ser: 
+ Diminuto: $0-5cm^{3}$ Ej: Reloj, Dado, Lápiz, etc.
+ Pequeño: $5-15cm^{3}$ Ej: Botella, Libro, Daga, etc. 
+ Mediano: $15-50cm^{3}$ Ej: Espada, Mochila, Bicicleta, etc.
+ Largo: $0.5-20m^{3}$ Ej: Estatua a tamaño real, Puerta, auto, etc.
+ Enorme: $20-50m^{3}$ Ej: Casa, aiuda no sé, etc.
+ Gigante: $50-150m^{3}$  Ej: Gran estatua, Templo, etc.

| Tamaño   | Cantidad de Dados |
| -------- | ----------------- |
| Diminuto | 1                 |
| Pequeño  | 2                 |
| Mediano  | 3                 |
| Largo    | 4                 |
| Enorme   | 5                 |
| Gigante  | 7                 |

> [!INFO] MÁS QUE GIGANTE
> 
> En el caso de que el objeto tenga un volumen mayor a Gigante se usará la siguiente fórmula:
> $$D(x)=2^{ \lceil x(150m^{3})^{-1} \rceil}+5$$
> Donde $x$ es el volumen del objeto.
> 
> Para simplificar, lo mejor será multiplicar la solución de la formula anterior por el resultado promedio del dado para obtener la cantidad de unidades de tiempo necesarias para completar el objeto.
### 4. Materiales y conocimientos necesarios
#### Materiales
Si no se tienen los materiales necesarios o una forma de conseguir los materiales necesarios para crear el objeto, no se puede completar el proceso. Para esto o se tienen todos los materiales e implementos de antemano o se tiene una tienda que provea materia prima en la cercanía, en el caso de este último será necesario disponer del dinero necesario para crearlos. Se puede referenciar la tabla de costos de DND para esto.
#### Conocimiento
También, el NPC debe tener conocimiento sobre el objeto que creará, no puede crear algo que no tiene idea de que se puede hacer o que no ha visto jamás. Entonces el conocimiento afecta la [[#3.Complejidad|complejidad]] de crear el objeto para el personaje, una guía puede ser:
+ No tiene idea de qué o cómo crear el objeto; Entonces no podrá crear el objeto.
+ Alguna vez a visto el objeto, pero no entiende completamente cómo funciona o cómo crearlo; Entonces es 1 categoría más compleja (Aquí afecta la [[#^e3ceec|experiencia previa]]).
+ Entiende el objeto o lo ha creado exitosamente antes; Entonces es de la categoría que corresponde.
> [!info] Experiencia previa
> Un personaje puede nunca haber creado este objeto en particular, pero ya haber creado un objeto similar en el pasado, o ya haber creado un mecanismo esencial. Entonces, al [[#5. Lanzar los dados y esperar|lanzar los dados]]  para obtener la cantidad de tiempo necesario, se lanzan con ventaja.
> 
> Un ejemplo sería construir una bicicleta por primera vez habiendo construido algo con pedales antes, entonces se tiene ventaja en la cantidad de días que tardará en construir la bicicleta. La ventaja quiere decir que se lanzan 2 veces los dados y se quedan con el mejor resultado. Supongamos que al lanzar 3d8 obtenemos \[8,1,5] en la primera ronda y \[4,4,1] en la segunda, entonces el mejor resultado es 9.

^e3ceec
### 5. Lanzar los dados y esperar
Una vez sabes la complejidad del objeto y el tamaño del mismo, sabes que dados lanzar y cuantos lanzar. Ahora solo queda lanzar los dados, sumar los resultados y esperar esa cantidad de tiempo "*in game*" para ver el resultado. 

Esta mecánica considera que el NPC trabaja 10 horas diarias en fabricar este objeto (en el caso de que la unidad de tiempo sea de días o mayor).
<div style="page-break-after: always;"></div>

> [!INFO] Proficiencias
> En el caso de que el personaje tenga proficiencia con las herramientas usadas para crear el objeto, se resta a cada tirada la proficiencia del personaje, o dicho de otra forma, al total de días se le resta la proficiencia multiplicado por la cantidad de dados lanzados.
### 6. Posibilidad de Fallar
Al esperar la cantidad de días necesarios para crear el objeto, hay una posibilidad de que éste falle al estar completo. Para calcular esta probabilidad se tiene en cuenta la complejidad del objeto que se fabricó y la cantidad de veces que el NPC ha fabricado este objeto. 
La probabilidad de éxito está dada por la ecuación:

$$P(x)=\lfloor(1-\frac{factor}{x+1})*100\rfloor$$
==La probabilidad de éxito mínima es de 40.==

Con $x$ la cantidad de veces que el NPC ha completado el objeto (ya haya fallado antes o haya tenido éxito), y $factor$ dado por la complejidad del objeto al momento de crearlo (teniendo en cuenta [[#^083e43|Habilidad Superior]]).

Una vez calculada la probabilidad de éxito, se lanzan los dados porcentuales (2d10), y si el resultado es menor igual o menor a la probabilidad calculada, entonces se tiene éxito y el objeto funciona a la perfección.

> [!Hammer] Reparar un resultado fallido
> Puedes dedicar $\lfloor\frac{t}{4}\rfloor$ (con mínimo 1) del tiempo dedicado a crear el objeto a repararlo, esta vez sin que el resultado falle, pero esta acción no suma otra vez a la cantidad de veces que el NPC a completado el objeto. 

> [!example] Ejemplo: Crear una Bicicleta
> Facktoré es una Gnomo que no tiene proficiencias, tiene tanto los materiales como las herramientas para crear una bicicleta y, aunque nunca ha creado una bicicleta antes sabe cómo hacerla.
>
>Una bicicleta es un objeto *"Mediano"* de complejidad *"Comprensible"*, por tanto debemos lanzar 3d8 para obtener la cantidad de días que se demorará Facktoré en fabricar una bicicleta.
>
>Obtenemos los siguientes resultados: \[1,2,6\], entonces Facktoré demorará 9 días en construir esta bicicleta.
>
>Una vez transcurridos los 9 días llega la hora de probar el resultado. Como Facktoré no ha construido una bicicleta antes, y la bicicleta tiene un factor de complejidad de 0.5, la probabilidad de Éxito es de:
>$$P(0)=\lfloor(1-\frac{0.5}{0+1})*100\rfloor=50$$
>Entonces si al lanzar los dados obtenemos un número menor o igual a 50, Facktoré ha tenido éxito y la bicicleta funciona. En el caso contrario, la bicicleta no funciona y tendrá que gastar otros $\lfloor9\div4\rfloor=2$ días en arreglar el resultado.
>
>Supongamos que al lanzar los dados obtenemos \[70,2\], es decir 72, por tanto la bici no funciona como debería y debe gastar otros 2 días arreglándola para tenerla funcional.
>
>Una vez transcurridos los 2 días extras, la bicicleta quedará totalmente funcional.
### Notas extras
#### A. Complejidades y Tamaños son Sugerencias
Tanto los tamaños como las complejidades son sugerencias, le DM decidirá en que categoría cae un objeto y este puede no cumplir con todas las características aquí descritas.
#### B. Posibilidad de que el objeto se rompa o descomponga
Considerar que un objeto hecho a mano quizás llega a descomponerse en un momento. Puedes tener esto en cuenta para objetos que rompan el balance del juego.