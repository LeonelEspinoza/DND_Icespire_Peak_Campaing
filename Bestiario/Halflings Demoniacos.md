---

---
#Enemigo #Halfling #Humanoide #StatBlock
{Imagen}
## Stat blocks
### Base
```statblock
statblock: true
name: "Halfling Demoniaco"
source: Homebrew
size: small
type: humanoid
subtype: Halfling (Stout)
alignment: Chaotic Evil
ac: 15
hp: 23
hit_dice: 5d6 + 5
speed: 30 ft.
modifier: +2
stats:
  - 14
  - 15
  - 13
  - 10
  - 10
  - 8
skillsaves:
  - Arcana: 2
  - Acrobatics: 5
  - Intimidation: 1
damage_vulnerabilities: radiant
damage_resistances: necrotic
damage_immunities: ""
condition_immunities: ""
senses: passive Perception 10
cr: 1/2
bestiary: true
traits:
  - name: Lucky
    desc: When rolling a 1 on an attack roll, ability check, or saving throw, you can reroll the die and must use the new roll.
    attack_bonus: 0
  - name: Brave.
    desc: Have advantage on saving throws against being [frightened](https://5e.tools/conditionsdiseases.html#frightened_phb).
    attack_bonus: 0
  - name: Halfling Nimbleness.
    desc: Can move through the space of any creature that is of a size larger than themselves.
  - name: Pack Tactics.
    desc: The halfling has advantage on an attack roll against a creature if at least one of the halfling's allies is within 5 feet of the creature and the ally isn't [incapacitated](https://5e.tools/conditionsdiseases.html#incapacitated_phb).
languages: Common, Halfling, Abyssal
actions:
  - name: Battleaxe (Two Hands)
    desc: _Melee Weapon Attack:_ +4 to hit, reach 5 ft., one target. _Hit:_ 7 (1d10 + 2) slashing damage.
    attack_bonus: 4
    hit_bonus: 2
creature: "Halfling Demoniaco"
```
### Guardia
```statblock
statblock: true
name: "Guardia Halfling Demoniaco"
source: Homebrew
size: small
type: humanoid
subtype: Halfling (Stout)
alignment: Chaotic Evil
ac: 17
hp: 33
hit_dice: 6d6 + 12
speed: 25 ft.
modifier: +1
stats:
  - 18
  - 12
  - 14
  - 10
  - 10
  - 8
skillsaves:
  - Arcana: 2
  - Athletics: 6
  - Intimidation: 1
damage_vulnerabilities: radiant
damage_resistances: necrotic
damage_immunities: ""
condition_immunities: ""
senses: passive Perception 10
cr: 1
bestiary: true
traits:
  - name: Lucky
    desc: When rolling a 1 on an attack roll, ability check, or saving throw, you can reroll the die and must use the new roll.
    attack_bonus: 0
  - name: Brave.
    desc: Have advantage on saving throws against being [frightened](https://5e.tools/conditionsdiseases.html#frightened_phb).
    attack_bonus: 0
  - name: Halfling Nimbleness.
    desc: Can move through the space of any creature that is of a size larger than themselves.
  - name: Pack Tactics.
    desc: The halfling has advantage on an attack roll against a creature if at least one of the halfling's allies is within 5 feet of the creature and the ally isn't [incapacitated](https://5e.tools/conditionsdiseases.html#incapacitated_phb).
languages: Common, Halfling, Abyssal
actions:
  - name: Multiattack.
    desc: The Halfling makes two Battleaxe attacks.
  - name: Battleaxe (One Hand)
    desc: _Melee Weapon Attack:_ +6 to hit, reach 5 ft., one target. _Hit:_ 7 (1d8 + 4) slashing damage.
    attack_bonus: +6 
    hit_bonus: +4
  - name: Battleaxe (Two Hands)
    desc: _Melee Weapon Attack:_ +6 to hit, reach 5 ft., one target. _Hit:_ 8 (1d10 + 4) slashing damage.
    attack_bonus: +6 
    hit_bonus: +4
creature: "Guardia Halfling Demoniaco"
```
### Explorador
```statblock
statblock: true
name: "Explorador Halfling Demoniaco"
source: Homebrew
size: small
type: humanoid
subtype: Halfling (Stout)
alignment: Chaotic Evil
ac: 15
hp: 27
hit_dice: 6d6 + 6
speed: 30 ft.
modifier: +4
stats:
  - 13
  - 18
  - 12
  - 10
  - 11
  - 8
skillsaves:
  - Arcana: 2
  - Acrobatics: 5
  - Intimidation: 1
damage_vulnerabilities: radiant
damage_resistances: necrotic
damage_immunities: ""
condition_immunities: ""
senses: passive Perception 10
cr: 1
bestiary: true
traits:
  - name: Lucky
    desc: When rolling a 1 on an attack roll, ability check, or saving throw, you can reroll the die and must use the new roll.
    attack_bonus: 0
  - name: Brave.
    desc: Have advantage on saving throws against being [frightened](https://5e.tools/conditionsdiseases.html#frightened_phb).
    attack_bonus: 0
  - name: Halfling Nimbleness.
    desc: Can move through the space of any creature that is of a size larger than themselves.
  - name: Agile.
    desc: Can dodge as a bonus action and Speed +5ft.
  - name: Pack Tactics.
    desc: The halfling has advantage on an attack roll against a creature if at least one of the halfling's allies is within 5 feet of the creature and the ally isn't [incapacitated](https://5e.tools/conditionsdiseases.html#incapacitated_phb).
languages: Common, Halfling, Abyssal
actions:
  - name: Shortsword/Scimitar.
    desc: _Melee Weapon Attack:_ +6 to hit, reach 5 ft., one target. _Hit:_ 7 (1d6 + 4) piercing/slashing damage.
    attack_bonus: 6
    hit_bonus: 4
  - name: Dagger.
    desc: _Melee or Ranged Weapon Attack:_ +6 to hit, reach 5 ft. or range 20/60 ft., one target. _Hit:_ 6 (1d4 + 4) piercing damage.
    attack_bonus: 6
    hit_bonus: 4
bonus_actions:
  - name: Shortsword/Scimitar.
    desc: _Melee Weapon Attack:_ +6 to hit, reach 5 ft., one target. _Hit:_ 3 (1d6) piercing/slashing damage.
    attack_bonus: 6
    hit_bonus: 0
  - name: Dagger.
    desc: _Melee or Ranged Weapon Attack:_ +6 to hit, reach 5 ft. or range 20/60 ft., one target. _Hit:_ 2 (1d4) piercing damage.
    attack_bonus: 5
    hit_bonus: 0
  - name: Dodge.
    desc: Agile feat.
    attack_bonus: 0
    hit_bonus: 0
creature: "Explorador Halfling Demoniaco"
```
## Feats
***
## Principales Características
Los Halflings demoniacos son un pueblo guerrero feroz, con ansias de conquistas que no tienen miedo de hacer pactos con entidades malignas con tal de saciar su sed de sangre. 

Debido al tiempo que han pasado relacionándose con entes demoniacos, su piel tiene un tono rojizo, fácilmente identificable; Además de lo anterior, deben mantenerse realizando sacrificios de sangre a dioses malignos con tal de no sufrir consecuencias rompiendo tratos antiguos. 

Está en su naturaleza la sed de sangre, pero hay quienes buscan redención y abandonan esta cultura o son exiliados por no ser parte del clan y cumplir con las expectativas. Aquellos que abandonan el clan, les es muy difícil no cometer crímenes o dañar a otras especies, es como si todos sus instintos les dirigieran a buscar hacer daño.
## Historia
Nadie recuerda el inicio del clan, hay leyendas antiguas sobre un guerrero Halfling embriagado de ira y en busca de venganza, realiza diversos pactos con entidades malignas, dándole la fuerza de combatir a todo aquel que se le cruce en su camino. 

Durante el último tiempo, la raza se ha enfocado en reunir armas mágicas y mantenerlas ocultas al exterior, con el objetivo de usarlas como carta de victoria con todo aquel que oponga resistencia a su agresividad. En un punto en su historia, los Halflings Demoniacos consiguen amasar una cantidad considerable de armas mágicas, utilizándolas como carta sorpresa contra cualquiera que tenga la mala suerte de ser atacado por ellos.

En un asedio a una fortaleza humana, al momento de utilizar su arma mágica como carta sorpresa se dan cuenta de las perfectas contramedidas hechas por el enemigo. Estas contramedidas no solo producen que la fortaleza humana salga victoriosa del asedio, si no que también terminan destruyendo varias de armas mágicas importantes en posesión de los Halflings demoniacos. Con el ardor de la derrota y la derrota todavía fresca, utilizan todos sus medios para encontrar la razón de la fuga de información, ¿Quién pudo haber ideado contramedidas perfectas para un arma que no saben como funciona? 

Al cabo de unos años, dan con el resultado, un Halfling del pantano era el causante de su vergüenza. Los frutos de la investigación apuntan a un cierto Halfling del pantano con la capacidad única de identificar el funcionamiento de armas mágicas con el simple hecho de tenerlas cerca. Este halfling habría estado relacionado con los humanos asediados, entregándoles información vital sobre el funcionamiento y el como defenderse de sus atacantes.

Ahora, con una rabia nacida de la venganza, buscan arrasar con aquellos capaces de arruinar sus cartas bajo la manga. Buscan exterminar a todos los Halflings de pantano. Es aquí donde comienza una guerra entre 2 pueblos de halflings.

Cuando [[Dio Rakitich]] tenía 30 años de edad, los Halflings Demoniacos arrasan con la aldea dejando muy pocos sobrevivientes. Creen que se han ganado la guerra y cumplido su objetivo: Exterminar a todos los Halflings del Pantano. Una vez terminan su guerra con los Halfling del Pantano, buscan aún más guerras en pos de llenar esa sed de sangre.

En la actualidad los Halflings demonios están distribuidos por todo el mundo, tanto en asentamientos pequeños como en ciudades, aunque debido a su naturaleza tan reactiva las grandes ciudades de Halflings demoniacos terminan quebrándose, por norma general se encuentran en agrupaciones/asentamientos medianos o pequeños. 

Recientemente ha llegado un grupo de Halflings demoniacos a las cercanías de [[Neverwinter]], una cantidad de 100 Halflings Demoniacos construyen un pequeño asentamiento para hacer de base de operaciones y poder mantener una guerra con otros pueblos y ciudades cercanas. Uno de los objetivos del asentamiento actualmente es reunir más armas mágicas y encontrar materiales con los cuales forjar armas mágicas dentro de las [[Colinas Metal de Estrella]].

***
## Cultura
En la cultura de los Halfling demoniacos, el dinero no tiene mucha presencia, suelen apreciar más a quienes tienen éxito en las batallas. Aquellos con una gran cantidad de reconocimientos en batalla se mantienen a base de otros Halflings demoniacos que buscan aprender de aquellos experimentados y reconocidos.

El color predominante al rededor de sus construcciones es el rojo.

La bandera que representa al pueblo de halflings demoniacos es una manta blanca manchada de sangre

Todo [[Halflings Demoniacos]] que se respete conoce la leyenda sobre el Halfling fundador, aquel que comenzó con este ciclo de sacrificios y sed de sangre. Lo alaban y rezan por algún día tener el poder que tuvo aquel que jamás fue derrotado.

En los asentamientos más grandes, conviven Halflings con otras criaturas demoniacas, en una relación simbiótica de confianza superficial.