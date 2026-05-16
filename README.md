# Robot quadrupède

| | |
|-|-|
|`Author` | Ben Haj Ayoub

## Description

## Motivation

## Architecture

### Block diagram

<!-- Make sure the path to the picture is correct -->
![Block Diagram](schematics/block_diagram.png)

### Schematic

![Schematic](schematics/kicad_schematic.png)

### Components


<!-- This is just an example, fill in with your actual components -->

| Device | Usage | Price |
|--------|--------|-------|
| Activ Buzzer | Buzzer | [1.5 RON](https://www.optimusdigital.ro/ro/audio-buzzere/635-buzzer-activ-de-3-v.html?search_query=buzzer&results=61) |
| Push Button | Button | [1 RON](https://www.optimusdigital.ro/ro/butoane-i-comutatoare/1119-buton-6x6x6.html?search_query=buton&results=222) |
| Jumper Wires | Connecting components | [7 RON](https://www.optimusdigital.ro/ro/fire-fire-mufate/884-set-fire-tata-tata-40p-10-cm.html?search_query=set+fire&results=110) |
| Breadboard | Project board | [10 RON](https://www.optimusdigital.ro/ro/prototipare-breadboard-uri/8-breadboard-830-points.html?search_query=breadboard&results=145) |

### Libraries

<!-- This is just an example, fill in the table with your actual components -->

| Library | Description | Usage |
|---------|-------------|-------|
| [lib-name1](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |
| [lib-name2](link-to-lib) | official description of the lib | Used for accesing the peripherals of the microcontroller  |

## Log

<!-- write every week your progress here -->

### Week 6 - 12 May

### Week 7 - 19 May

### Week 20 - 26 May# Robot quadrupède

| | |
|-|-|
|`Author` | Ben Haj Ayoub |

## Description
Ce projet consiste à construire un robot quadrupède (robot araignée) basé sur la carte de développement Arduino Nano. Le robot utilise 12 micro servomoteurs pour articuler ses jambes de manière fluide, un capteur à ultrasons pour éviter les obstacles de manière autonome, et est alimenté par deux batteries 18650 via un régulateur de tension.

## Motivation
Créer un robot marcheur fonctionnel pour mettre en pratique la programmation C++, explorer la cinématique des servomoteurs, et gérer l'alimentation embarquée d'un système complexe.

## Architecture

### Block diagram

![Block Diagram](schematics/block_diagram.png)

### Schematic

![Schematic](schematics/kicad_schematic.png)

### Components

| Device | Usage | Price (Unit. fără TVA) |
|--------|--------|-------|
| Micro Servomotor SG90 90° (x12) | Mouvement des articulations du robot | 11.56 RON |
| Placă de Dezvoltare Arduino Nano (ATmega328p) | Microcontrôleur principal | 24.26 RON |
| Placă de Expansiune pentru Arduino Nano | Shield pour faciliter les connexions des servos | 6.45 RON |
| Suport de Baterii 2 x 18650 | Support pour l'alimentation | 3.30 RON |
| Sursa Coboratoare de Tensiune LM2596 (5V) | Régulateur de tension pour protéger les composants | 10.74 RON |
| Senzor Ultrasonic HC-SR04+ | Détection d'obstacles (3.3V / 5V) | 12.39 RON |
| Acumulator Murata US18650VTC5C 2600mAh (x2) | Alimentation de puissance pour le robot | 18.18 RON |
| Set 10 Fire Colorate Mamă-Mamă 10 cm (x2) | Câblage électronique général | 2.69 RON |
| Intrerupator Negru On/Off | Contrôle de l'alimentation principale | 0.82 RON |
| Set 6 Șurubelnițe în Miniatură | Outils pour l'assemblage mécanique | 4.12 RON |

### Libraries

| Library | Description | Usage |
|---------|-------------|-------|
| [Servo.h](https://www.arduino.cc/reference/en/libraries/servo/) | Official Arduino Servo Library | Utilisée pour le contrôle individuel des 12 servomoteurs SG90. |
| [FlexiTimer2.h](https://playground.arduino.cc/Main/FlexiTimer2/) | Timer interrupt library | Utilisée pour gérer la synchronisation précise du temps et la coordination de la marche de l'araignée. |

## Log

### Week 6 - 12 May
* Réception des composants matériels.
* Début de l'assemblage physique du châssis du robot quadrupède et montage des 12 servomoteurs.

### Week 7 - 19 May
* Câblage de l'électronique : mise en place de la plaque d'expansion avec l'Arduino Nano, intégration du LM2596 pour la conversion 5V, et connexion du HC-SR04.
* Écriture des premiers scripts de test pour calibrer les servomoteurs SG90.

### Week 20 - 26 May
* Implémentation du code C++ principal avec l'intégration de la bibliothèque FlexiTimer2.
* Ajustements de la cinématique pour stabiliser la marche et tests de la logique d'évitement d'obstacles.


## Reference links

<!-- Fill in with appropriate links and link titles -->

[Tutorial 1](https://www.youtube.com/watch?v=wdgULBpRoXk&t=1s&ab_channel=BenEater)

[Article 1](https://www.explainthatstuff.com/induction-motors.html)

[Link title](https://projecthub.arduino.cc/)
