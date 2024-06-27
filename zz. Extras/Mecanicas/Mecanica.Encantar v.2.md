#Sistema de Polito inspirado en Heliana's Guide to Monster Hunter
<center> <h1> Mecánica Homebrew: <br> Encantar </h1></center>

# ¿Qué es?
Encantar es imbuir objetos con magia extraída de otras criaturas mágicas, dandole distintas propiedades. Este sistema está pensado principalmente para armas, armaduras y objetos de aventureros, pero puede usarse para lo que el DM permita.

Encantar solo puede ser usado por spellcasters o seres afines a lo arcano.
***
# **Materiales**
Los materiales necesarios para encantar son:
+ Objeto a encantar
+ Formula del encantamiento
+ Componente mágico
+ Oro 
+ Esencia.
## **Formula del Encantamiento**
Se ocupan para entender cómo encantar un objeto. Esta indica cuales son los materiales, oro y esencias necesarias para el proceso. Es posible encontrar estas formulas y/o comprarlas.
#### Crear una formula a partir de un objeto mágico
Un spellcaster con un modificador de Investigación y arcana mayor a 0 puede estudiar un objeto  mágico para obtener la formula de su encantamiento. El tiempo que requiere esto esta dado por la siguiente tabla:

| Calidad del Objeto | Dekhanas |
| :----------------: | :------: |
|       Común        |    1     |
|      No común      |    2     |
|        Raro        |    5     |
|      Muy Raro      |    10    |
|     Legendario     |    20    |
|     Artefacto      |    50    |
#### Encantar sin formula
Se puede intentar encantar un objeto sin su formula, pero hay una penalización de -50 al check final para obtener el resultado.
## **Componente Mágico**
Para encantar un objeto es necesario algún componente mágico que permita darle las propiedades mágicas que se buscan en un objeto. El componente mágico debería estar relacionado con el efecto que se busca en el resultado final.

> [!Example] **Por ejemplo**:
> Para una daga de fuego es necesario escamas de dragón rojo. 

#### Buscar y comprar los componentes
Está la opción de buscar los elementos necesarios en el comercio de los asentamientos como pueblos o ciudades, y estos pueden ser comprados gastando dinero.

Es importante considerar que no cualquier asentamiento tiene los materiales para encantar. Puede que simplemente no se encuentren los objetos que buscan en los alrededores.

| Calidad    | Oro         | Tiempo Buscando |
| ---------- | ----------- | --------------- |
| Común      | 1d4x10gp    | 1 semana        |
| No común   | 2d6x10gp    | 2 semanas       |
| Raro       | 1d10x100gp  | 3 semanas       |
| Muy Raro   | 1d6x1000gp  | 5 semanas       |
| Legendario | 2d10x1000gp | 7 semanas       |
| Artefacto  | 2d20x1000gp | 10 semanas      |
#### Catalizadores
En vez de ser un componente específico, puede utilizarse un catalizador. Un catalizador es un objeto capaz de contener "magia" para imbuir un objeto.

Utilizando el [[Mecanica.Crear_Objetos|sistema de creación]]:
+ Tamaño: depende del objeto a encantar, pero es básicamente un tamaño más chico que el objeto. 
+ Dificultad: la dificultad para construir el catalizador depende de la rareza del objeto, y está dada por la siguiente tabla: 

| Rareza     | Complejidad       |
| ---------- | ----------------- |
| Común      | Simple            |
| No Común   | Comprensible      |
| Raro       | Confuso           |
| Muy Raro   | Complejo          |
| Legendario | Técnico           |
| Artefacto  | Sumamente Técnico |

## **Oro**
El oro funciona como conductor de la magia. Se requiere una cantidad de oro proporcional a la calidad del objeto mágico para poder llevar a cabo el proceso de encantamiento de un objeto.

| Calidad    | Oro necesario |
| ---------- | ------------- |
| Común      | 10gp          |
| No común   | 100gp         |
| Raro       | 400gp         |
| Muy Raro   | 1000gp        |
| Legendario | 5000gp        |
| Artefacto  | 25000gp       |

> [!Info] Precio de Venta
> Un objeto mágico usualmente se vende por 1.5 veces la cantidad de oro que se utiliza para encantarlo. 

## **Esencia**
Un componente mágico que se puede recolectar de las criaturas caídas dependiendo de su CR.
La esencia determina la rareza del objeto imbuido según la siguiente tabla:

| Rareza del Encantamiento | Poder de la Esencia |  CR   |
| :----------------------: | :-----------------: | :---: |
|          Común           |          -          |   -   |
|         No común         |       Frágil        |  3-6  |
|           Raro           |       Robusto       | 7-11  |
|         Muy Raro         |       Potente       | 12-17 |
|        Legendario        |       Mítico        | 18-24 |
|        Artefacto         |       Deífico       |  25+  |

# Tiempo Necesario
Teniendo todos los materiales necesarios para comenzar a encantar el objeto, se puede determinar cuanto tiempo demorará encantar el objeto. Para determinar el tiempo que tarda realizar el encantamiento es necesario lanzar dados y multiplicar el resultado por un factor $Chrono$ ; Los dados y el factor $Chrono$ está determinado por la rareza del encantamiento según la siguiente tabla:

| Rareza del Encantamiento | Dado | Chrono |
| :----------------------: | :--: | ------ |
|          Común           |  d1  | 1      |
|         No común         |  d4  | 2      |
|           Raro           | d10  | 3      |
|         Muy Raro         | d20  | 5      |
|        Legendario        | 2d20 | 7      |
|        Artefacto         | 5d20 | 10     |
Una vez se lanzan los dados, el tiempo que tarda esta dado por la siguiente formula:
$$Tiempo=Dado*Chrono$$

> [!info] Notas
> + El tiempo está medido en días, y se considera que se gastan 12 horas diarias encantando. Es decir, pasan la mayor parte del día encantando el objeto.
> + Si el objeto que se va a crear es un consumible, el tiempo de creación se divide en 3


# Resultado
Una vez transcurrido el tiempo necesario para completar el encantamiento, es hora de verificar el éxito o fallo del mismo. El check para el éxito del encantamiento tiene un DC determinado por la siguiente función:
$$DC= Dificultad* \frac{1}{z+1}$$
Con $z$ siendo la cantidad de veces que el personaje ha intentado encantar este objeto, y la $Dificultad$ es dependiente de la rareza del encantamiento, determinada por la siguiente tabla:

| Rareza del Encantamiento | Dificultad |
| :----------------------: | :--------: |
|          Común           |     20     |
|         No común         |     40     |
|           Raro           |     60     |
|         Muy Raro         |     80     |
|        Legendario        |    100     |
|        Artefacto         |    120     |
Una vez se calcula el DC, es hora de tirar un dado porcentual, y al resultado del dado se le suma 5 veces el modificador de la habilidad de spellcasting. Es decir, el check tiene éxito solo sí:
$$1d100\ + 5*Ability\ Modifier \ge DC$$
En caso de tener proficiency en arcana se agrega el proficiency bonus al modificador de habilidad de spellcasting, quedando:
$$1d100\ + 5*(Ability\ Modifier\ +Proficiency\ Bonus) \ge DC$$
Fallar el check significa que fallo el encantamiento y hay que comenzar desde 0 para poder intentarlo de nuevo.
# Extras
## Expertos y Maestros
si el objeto lo hacen con una persona que es experta en el tipo de encantamiento que están buscando tienen distintas ventajas. La categoría en la que entra este experto depende netamente del DM

| Experto     | Velocidad | Bonus para el DC | Costo por Hora |
| ----------- | --------- | ---------------- | -------------- |
| Amateur     | x1        | +15              | 20gp           |
| Profesional | x2        | +30              | 80gp           |
| Maestro     | x3        | +50              | 180gp          |
## Bonus y Penalizaciones
Fallar el check, cuando se habla de encantamiento, no necesariamente significa que no se pueda encantar, sino que el encantamiento no funcionó como debería. Esto ocurre cuando los dados que salieron en la tirada no fueron los deseados pero se estuvo muy cerca de lograr el encantamiento, entonces se logra encantar pero con una penalización.
Lo mismo ocurre hacia el otro lado, si se logra sacar números muy altos en un check bajo, lo más probable es que se puedan sacar un objeto con encantamientos muy poderosos. Pero esto también está condicionado a la rareza del encantamiento, un objeto común no se puede esperar que sea demasiado poderoso si no se le ha imbuido ninguna esencia. La cantidad de bonificaciones se puede ver en la siguiente tabla:

|   Rareza   | Máx. de Fallas o Bonus |
| :--------: | :--------------------: |
|   Común    |           0            |
|  No Común  |           1            |
|    Raro    |           2            |
|  Muy Raro  |           3            |
| Legendario |           3            |
| Artefacto  |           3            |
Para determinar si logra conseguir o bonificaciones o penalizaciones, depende del DC sacado y la diferencia de este con respecto a el DC esperado se tiene que observar la siguiente tabla:

| Diferencia con el DC | Resultado                                   |
| :------------------: | ------------------------------------------- |
|     -41 o menos      | Fracaso total, el encantamiento no funciona |
|      -31 a -40       | 3 Fallas                                    |
|      -16 a -30       | 2 Fallas                                    |
|       -1 a -15       | 1 Falla                                     |
|        0 a 15        | Nada                                        |
|       16 a 30        | 1 Bonus                                     |
|       31 a 40        | 2 Bonus                                     |
|       41 o más       | 3 Bonus                                     |
En el caso de los objetos que solo tengan un máximo de fallas, la siguiente falla sería contada como fracaso total. Por ejemplo, se está creando un objeto  de rareza "No común". El DC para esto es 40 y tiene un máximo de fallas de 1, si se saca una diferencia negativa con el DC de más de 15, entonces el encantamiento no funciona, ya que se consideraría que tiene "2 fallas", pero el máximo era solo 1.

En el caso de no funcionar, todos los elementos usados, menos el objeto (oro, esencia y materiales mágicos), son gastados y no se pueden recuperar del proceso.

Para determinar que falla o bonus tocó, se puede revisar la siguiente tabla, para la cual se pide lanzar un d20 y revisar que sale.
En el caso de que salga el mismo número dos veces en la tabla, se vuelve a rolear hasta que salga algo distinto.
#### Tabla de Penalizaciones

| d20  | Falla                   | Descripción                                                                                                                                                                                                                                     |
| ---- | ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1-2  | Maldito                 | El objeto se vuelve maldito y no lo puedes despegar de ti a menos que lo destroces. Para ver la maldición vuelve a lanzar el dado y esa será la maldición.                                                                                      |
| 3    | Rabia de Batalla        | Cuando se termine el combate tienes que superar un check de sabiduría DC10 a menos que seas inmune al encantamiento. En el caso de fallar ve a todas las criaturas como enemigas y las ataca. En su turno tiene que volver a hacer el mismo ST. |
| 4    | Insensibilidad          | Todo se vuelve blanco y negro. Darkvision se reduce en 30ft. Nada huele ni sabe a nada. Sonidos se escuchan como si estuviesen debajo del agua. Todo lo que tocas se siente como hormigas y tienes desventaja en checks de Perception           |
| 5    | Pozo de Gravedad        | Pesas 3 veces lo que deberías pesar y tu velocidad se reduce en 5ft                                                                                                                                                                             |
| 6    | Falsedad                | Cada vez que dices la verdad, tomas 1d6 de daño psiquico. Esto no ocurre más de una vez por minuto.                                                                                                                                             |
| 7    | Encontrable             | Cualquier criatura con proficiencia en Arcana que esté en tu mismo plano puede usar una acción para determinar tu posición exacta.                                                                                                              |
| 8    | Analfabeta              | No puedes ni leer ni escribir                                                                                                                                                                                                                   |
| 9    | Atracción               | Ataques a distancia tienen ventaja cuando van hacia ti                                                                                                                                                                                          |
| 10   | Imán                    | Spells, ataques y efectos que hagan un tipo de daño especifico tienen ventaja cuando van contra ti                                                                                                                                              |
| 11   | Miedo Primal            | Haces la mitad de daño contra bestias                                                                                                                                                                                                           |
| 12   | Monologo Externo        | Cada vez que termines un long rest, tienes que hacer un Saving Throw de Sabiduría o ser maldito. Mientras tengas esta maldición, tienes que decir todos tus pensamientos en voz alta hasta que vuelvas a hacer el ST después de un Long Rest    |
| 13   | Reacción en Cadena      | Cuando sufres daño de un tipo dictado por el DM, sufres 3d6 y todas las criaturas a 10ft de ti tienen que hacer un Dex Saving Throw. En caso de fallar toman 3d6 de daño                                                                        |
| 14   | Descomposición          | Te ves como si te has podrido y decaído por días. Otras criaturas con excepción de no muertas tienen miedo. Tienes ventaja en checks de Intimidación pero desventaja en todos los demás checks de Carísma                                       |
| 15   | Conservación deficiente | Cuando sufres un golpe crítico, tienes que realizar un Con Saving Throw. En caso de fallar te conviertes en una criatura de CR0 elegida por el DM por 1 hora.                                                                                   |
| 16   | Ingenuo                 | Desventaja en todos los checks de Insight                                                                                                                                                                                                       |
| 17   | Marcado                 | Las criaturas de un tipo en especifico dictado por el DM querrán este item. Si están a 300ft de tí sabrán tu ubicación exacta y te la querrán comprar, robar o quitar a la fuerza.                                                              |
| 18   | Veracidad               | Cada vez que dices una mentira, tomas 1d6 de daño psiquico. Este efecto no puede ocurrar más de una vez por minuto                                                                                                                              |
| 19   | Potencia Alcoholica     | Cada vez que consumes un liquido mágico se siente como si fuese alcohol. Tienes que realizar un Con Saving Throw. En caso de fallar te emborrachas y tienes desventaja en attack rolls.                                                         |
| 20   | Emparejamiento Forzado  | Este objeto ahora está ligado a tí y no puedes ponerte otros objetos que requieran attunement. Para remover esto tienes que completar una misión dada por el objeto mágico que será dictada por el DM                                           |
#### Tabla de Bonus

| Dado | Nombre                  | Bonus                                                                                                                                                                                                                                     |
| ---- | ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | Pelología               | Puedes cambiar el color de tu pelo del color que quieras, lo cual dura 1 minuto.                                                                                                                                                          |
| 2    | Feromonas ventajosas    | Emites un odor especial para las bestias y otras criaturas simples. Tienes ventaja en todos los checks de Animal Handling                                                                                                                 |
| 3    | Ludopata                | Tienes un gran entendimiento de todos los juegos de azar. Ganas proficiencia en todos los gaming sets                                                                                                                                     |
| 4    | Vacío de gravedad       | Cuando te caes, te puedes levantar usando 5ft                                                                                                                                                                                             |
| 5    | Escape                  | Tu velocidad aumenta en 5ft                                                                                                                                                                                                               |
| 6    | Compuesto               | La magia de ilusión cubre cualquier falla que puedes tener. Tienes ventaja en todos los checks de Deception                                                                                                                               |
| 7    | Geolocalicación         | Siempre sabes cual dirección es norte. Además, siempre sabes si estás por sobre o bajo el nivel del mar.                                                                                                                                  |
| 8    | Rayo del sol            | Como bonus action, puedes ccrear una luz que ilumina un radio de 20ft y crea iluminación leve en los siguientes 20ft.                                                                                                                     |
| 9    | Caída de gato           | Recibes la mitad del daño al caer                                                                                                                                                                                                         |
| 10   | Ojos de la debilidad    | Como bonus action puedes identificar cuales son los Saving Throw más debiles de una criatura                                                                                                                                              |
| 11   | Proficiente             | El item te agrega sabiduría en un ambito. Ganas proficiencia en una skill.                                                                                                                                                                |
| 12   | Sustancia               | Requieres la mitad de la comida y el agua de lo que normalmente necesitas. Además, cada vez que eres curado por magia, puedes rolear de nuevo si te sale un 1.                                                                            |
| 13   | Asesino de criaturas    | Ataques que hagas contra cierto tipo de criaturas hacen daño extra igual a tu proficiencia                                                                                                                                                |
| 14   | Intuitivo               | Tienes una habilidad para determinar si alguien te está mintiendo. Tienes ventaja en Insight checks para determinar si alguien miente                                                                                                     |
| 15   | Refinador de oxigeno    | Puedes respirar bajo el agua                                                                                                                                                                                                              |
| 16   | Repulsor de energía     | Spells, ataques que hagan un tipo de ataque específico tienen desventaja contra ti. Y tu tienes ventaja en Saving Throws para resistirlos                                                                                                 |
| 17   | Sistema de conservación | Cada vez que eres golpeado con un crítico, puedes ocupar tu reacción para convertir al atacante en una criatura de CR igual a tu proficiencia. Solo puede ser usado una vez por día y contra criaturas del mismo o menor CR que tu nivel. |
| 18   | Sidekick                | Eres bueno dando apoyo. Cuando usas la acción de ayudar, la otra criatura recibe 1d4 a su roll.                                                                                                                                           |
| 19   | Poder                   | Tienes +1 en rolls de ataque y en el DC de spellcasting                                                                                                                                                                                   |
| 20   | Compromiso extra        | La cantidad de objetos a los que te puedes comprometer (attunement) aumenta en 1                                                                                                                                                          |
# Créditos
Tanto esta tabla como la de bonus fue creada por otra persona y se puede encontrar en: Heliana's Guide to Monster Hunter