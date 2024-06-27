#Sistema de Leo y Polito
<center> <h1> Mecánica Homebrew: <br>Tiempo de Creación de Objetos </h1></center>

## ¿Qué es?

Ésta mecánica cumple el propósito de poder crear objetos con algún NPC que esté habilitado para esto. Principalmente indica cuanto tiempo se demorará el NPC en conseguir un resultado, el cual tiene una posibilidad de fallar.
## ¿Cómo funciona?
#### 1. **Elegir objeto a crear**:
Lo primero es seleccionar el objeto que se busca crear. Esto puede ser un objeto que ya  exista en DND o puede ser algo externo. En el caso de que ya exista, lo recomendable será tomar en cuenta sus estadísticas. El objeto determina que tan complejo es y que tamaño tendrá  
#### 2. **Complejidad**:
Que tan complejo es un objeto determina el tipo de dado que se usa para definir cuánto tiempo se tarda en crearlo.

|  **Complejidad**  |    **Dado**     | **Factor** |
| :---------------: | :-------------: | :--------: |
|      Trivial      | $\frac{d4}{20}$ |     5      |
|     Sencillo      | $\frac{d4}{10}$ |     10     |
|      Simple       |      $d4$       |     15     |
|    Compensible    |      $d6$       |     20     |
|      Confuso      |      $d10$      |     30     |
|     Complejo      |      $d20$      |     40     |
|      Técnico      |     $2d20$      |     60     |
| Sumamente Técnico |     $10d20$     |     80     |
#### 3. **Tamaño:**
El tamaño de un objeto indica el factor utilizado para determinar la cantidad de días. Los tamaños pueden ser:

| **Tamaño** |       **Medidas**        | **Multiplicador** |          Ejemplo           |
| :--------: | :----------------------: | :---------------: | :------------------------: |
|  Diminuto  |       0 - 5x5x5cm        |        0,5        |        Reloj, Lápiz        |
|  Pequeño   |   5x5x5cm - 15x15x15cm   |         1         |       Botella. Libro       |
|  Mediano   | 15x15x15cm - 50x50x50cm  |         2         | Espada, Mochila, Bicicleta |
|   Grande   |  50x50x50cm - 5mx5mx5m   |         4         |        Auto, Puerta        |
|   Enorme   |    5x5x5m - 25x25x25m    |        10         |            Casa            |
|  Gigante   | 25x25x25m - 150x150x150m |        20         |     Castillo, Estatua      |

^6289cf

> [!INFO] *Más que Gigante:*
> En el caso de que el objeto tenga un volumen mayor a Gigante, se usará la siguiente fórmula:
>
>$$D(x) = 2^{\lceil x/(150)\rceil} + 18$$
>
>Donde $x$ es el largo promedio del objeto.
>
>Para simplificar, lo mejor será multiplicar la solución de la formula anterior por el resultado promedio del dado para obtener la cantidad de unidades de tiempo necesarias para completar el objeto.
#### 4. **Materiales y Conocimientos necesarios**
- **Materiales**: 
	Si no se tienen los materiales necesarios o una forma de conseguir los materiales necesarios para crear el objeto, no se puede completar el proceso. Para esto o se tienen todos los materiales e implementos de antemano o se tiene un proveedor de materia prima en la cercanía, en el caso de este último será necesario disponer del dinero necesario para crearlos. Se puede referenciar la tabla de costos de DND para esto.

- **Conocimiento**: 
	También, el NPC debe tener conocimiento sobre el objeto que creará, no puede crear algo que no tiene idea de que se puede hacer o que no ha visto jamás. Entonces el conocimiento afecta la complejidad de crear el objeto para el personaje, una guía puede ser:
	- **No tiene idea de qué o cómo crear el objeto**: No se podrá crear el objeto
	- **Alguna vez ha visto el objeto:** Entonces es 1 categoría más compleja (Aquí afecta la experiencia previa)
	- **Entiende el objeto y lo ha creado exitosamente antes:** Es de la categoría que le corresponde.
	

> [!Info] *Experiencia previa*:
>  Un personaje puede nunca haber creado este objeto en particular, pero ya haber creado un objeto similar en el pasado, o ya haber creado un mecanismo esencial. Entonces, al lanzar los dados para obtener la cantidad de tiempo necesario, se lanzan con ventaja. Un ejemplo sería construir una bicicleta por primera vez habiendo construido algo con pedales antes, entonces se tiene ventaja en la cantidad de días que tardará en construir la bicicleta. La ventaja quiere decir que se lanzan 2 veces los dados y se quedan con el mejor resultado. 
#### 5. **Lanzar los dados y esperar**:
Una vez sabes la complejidad del objeto y el tamaño del mismo, sabes que dados y cuantos lanzar. Ahora solo queda sumar o multiplicar los resultados con la siguiente formula para calcular tiempo final es:
$$Tiempo = Dado * Multiplicador$$
 y esperar esa cantidad de tiempo *"in game"* para ver el resultado.
 
> [!NOTE] Notas:
> - El [[#^6289cf|multiplicador]] puede cambiarse por cantidad de dados antes de lanzar.
> - El tiempo está medido en días, y si se quiere llevar a horas: 1 día = 12 horas trabajando

> [!NOTE] *Proficiencias:*
> En el caso de que el personaje tenga proficiencia con las herramientas usadas para crear el objeto, se resta a cada tirada la proficiencia del personaje, o dicho de otra forma, al total de días se le resta la proficiencia multiplicado por la cantidad de dados lanzados.
#### 6. **Posibilidad de fallar:**
Al esperar la cantidad de días necesarios para crear el objeto, hay una posibilidad de que éste falle al estar completo. Para calcular la dificultad de éxito se tiene en cuenta la complejidad del objeto que se fabricó y la cantidad de veces que el NPC ha fabricado este objeto.  
La probabilidad de éxito está dada por la ecuación:

$$DC = \frac{factor}{z+1}$$

Con $z$ la cantidad de veces que el NPC ha completado el objeto(ya haya fallado antes o haya tenido éxito), y el $factor$ dado por la complejidad del objeto al momento de crearlo.

Una vez calculado el DC, se lanza el d100, y si el resultado es mayor o igual a la probabilidad calculada, entonces se tiene éxito y el objeto funciona a la perfección.

Puedes dedicar $\lfloor t/4\rfloor$ (con mínimo 1) del tiempo dedicado a crear el objeto a repararlo, esta vez sin que el resultado falle, pero esta acción no suma otra vez a la  cantidad de veces que el NPC a completado el objeto.
#### **Expertiz**
Si este proceso es hecho por gente que tiene experiencia en el tema y que de cierta forma son expertos en el proceso de creación, tienen distintas ventajas:

| Expertiz    | Aumento de velocidad | Bonus para el DC |
| ----------- | -------------------- | ---------------- |
| Amateur     | x1                   | +15              |
| Profesional | x2                   | +30              |
| Maestro     | x3                   | +50              |

## **Ejemplo: Crear una bicicleta**
Facktoré es una Gnomo que no tiene proficiencias, tiene tanto los materiales como  
las herramientas para crear una bicicleta y, aunque nunca ha creado una bicicleta  
antes sabe cómo hacerla.

Una bicicleta es un objeto "Mediano" de complejidad "Comprensible", por tanto  
debemos lanzar 2d6 o 1d6 y multiplicar por 2 para obtener la cantidad de días que se demorará Facktoré en  fabricar una bicicleta. Obtenemos los siguientes resultados: \[2,6], entonces Facktoré demorará 8 días en construir esta bicicleta.  

Transcurridos los 8 días llega la hora de probar el resultado. Como Facktoré no ha construido una bicicleta antes, y la bicicleta tiene un factor de complejidad de 40 la probabilidad de Éxito es de:

$DC = \frac{40}{1} = 40$

Entonces si al lanzar los dados obtenemos un número mayor o igual a 40, Facktoré ha tenido éxito y la bicicleta funciona. En el caso contrario, la bicicleta no funciona y tendrá que gastar otros $\lfloor 8/4\rfloor = 2$ días en arreglar el resultado. Supongamos que al lanzar el d100 obtenemos 28, por tanto la bici no funciona como debería y debe gastar otros 2 días arreglándola para tenerla  
funcional. 

Transcurridos los 2 días extras, la bicicleta quedará totalmente funcional.
## **Notas Extra**
- **Complejidad y tamaño son sugerencias:** Tanto los tamaños como las complejidades son sugerencias, le DM decidirá en que categoría cae un objeto y este puede no cumplir con todas las características aquí descritas.
- **Posibilidad de que el objeto se rompa o descomponga:** Considerar que un objeto hecho a mano quizás llega a descomponerse en un momento. Puedes tener esto en cuenta para objetos que rompan el balance del juego.

