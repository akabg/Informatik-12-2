# Informatik-12.2

## Inhaltsverzeichnis

[Unser Projekt](#1)

[Blog](#2)

[Fazit](#3)

[Finale Links](#4)

### <a name="1"></a>Unser Projekt

<details>
<summary>Vorstellung</summary>
<br>
Unsere Gruppe, bestehend aus Antonia, Farhat und Vanessa hat ein Spiel namens 'CatchCorona' programmiert. 
Die Idee des Spiels ist es, dass der Spieler einen Antikörper steuert. Dabei muss er mit Hilfe der Pfeiltasten das Coronavirus jagen. Wenn der Antikörper das Virus berührt, hat der Spieler gewonnen. Um die Schwierigkeiten zu erhöhen gibt es auch Hindernisse, denen man ausweichen muss, oder die auf einen schießen, die Aluhüte. Letztendlich hat man auch nur eine bestimmte Zeit zum einfangen, da ein Timer runterläuft.
Programmiert haben wir mit Greenfoot, eine interaktive Java-Entwicklungsumgebung. Dies war für alle in der Gruppe das erste "echte" programmieren.
</details>


<details>
<summary>Aufbau</summary>
<br>

### 1. Start Screen
Wenn man das Spiel startet, trifft man als erste auf den StartScreen. Wenn man den StartButton drückt, verschwindet er und stattdessen wird eine Spritze in die Welt gesetzt, die die Impfung darstellen soll. Zusätzlich wird der Schriftzug "Hilfe, rette mich vor Corona!" angezeigt. 
Die Spritze bewegt sich über den Bildschirm nach links und setzt auf halben Wege ein Anitkörper (das der Spiler später steuert) in die Welt. Wenn es den Rand des Screens berührt, wird der GameScreen geöffnet.
 
### 2. Game Screen
Hier beginnt das eigentliche Spiel. Das zu fangende Objekt, Corona, fängt sofort an sich zufällig über den Bildschirm zu bewegen. Der zu steuernde Antikörper fängt erst an sich zu bewegen und sich steuern zu lassen, wenn man die Eingabetaste drückt. Auch die Hindernisse spawnen direkt.
Man spielt jetzt also klassisch das Spiel und versucht dabei nicht zu sterben und im Rahmen der Zeit Corona zu fangen.
Am Ende des Spiels öffnet sich je nach Ausgang, entweder der Win-Screen oder der Loose-Screen.

### 3.1 Win-Screen
Du gewinnst, wenn Antikörper Corona berührt.

### 3.2 Loose-Screen
Du landest hier wenn:
- Antikörper Alu berührt
- Antikörper abgeschossen wird
- der Timer abgelaufen ist
 
  
</details>

<details>
<summary> World (Setting) </summary>
<br>
 
Es gibt 4 verschiedene Screens/worlds. Ein Start Screen, ein GameScreen und jeweils ein loose/win Screen. Alle spielen in einer Ader, also im menschlichen Blutkreislauf.

### 1. Start Screen
 
Inhalt
- StartButton
- Schriftzüge
- Spritze
- Nicht steuerbarer Antikörper
 
<p align="center">
<img width="600" alt="Start1" src="https://user-images.githubusercontent.com/88386173/162732710-16f9ecd8-2ec9-441d-b9e2-3fdacdb7a9f7.JPG" />
</p>
 
<p align="center">
<img width="600" alt="Start2" src="https://user-images.githubusercontent.com/88386173/162732774-652f01ce-be59-40f8-bc7e-e4e4ca494a82.JPG" />
</p>
 
<p align="center">
<img width="600" alt="StartCode" src="https://user-images.githubusercontent.com/88386173/162732566-2f1e340e-3cff-49ef-9142-7c3ed5ca5f09.JPG" />
</p>
 

### 2. Game Screen
 
Inhalt:
- Timer
- Antikörper (steuerbar)
- Corona
- Aluhüte (spawnen random)
- Shooter
- Shot
 
<p align="center">
<img width="600" alt="Game" src="https://user-images.githubusercontent.com/88386173/162733248-0f84099c-1577-4982-945e-fe17ad2e494b.JPG" />
</p>

<p align="center">
<img width="600" alt="GameCode1" src="https://user-images.githubusercontent.com/88386173/162732820-c555a8bd-6422-485e-84c5-cc7accb92781.JPG" />
</p>
 
<p align="center">
<img width="450" alt="GameCode2" src="https://user-images.githubusercontent.com/88386173/162732826-74bb813f-fe82-4aee-89f5-fb88f6a78226.JPG" />
</p>

### 3.1 Win-Screen

Inhalt:
- Play Again Button
 
<p align="center">
<img width="600" alt="WinScreen" src="https://user-images.githubusercontent.com/88386173/162733304-6e2137d5-6c3d-4857-b5af-a16113942233.JPG" />
</p>

<p align="center">
<img width="600" alt="WinCode" src="https://user-images.githubusercontent.com/88386173/162733374-dec407f3-642c-4ce3-9b10-353630161b58.JPG" />
</p>

### 3.2 Loose-Screen

Inhalt:
- Play Again Button
 
<p align="center">
<img width="600" alt="LooseScreen" src="https://user-images.githubusercontent.com/88386173/162733471-60b75e3f-29fe-4ffb-afa8-8c5e7f1c7b6e.JPG" />
</p>

<p align="center">
<img width="600" alt="LooseCode" src="https://user-images.githubusercontent.com/88386173/162733477-9566d2a9-58e8-4f43-93fb-46c7b41a2a63.JPG" />
</p>

 </details>


<details>
<summary>Actors</summary>
<br>
 
 <p align="center">
  <img width="100" alt="Actors" src="https://user-images.githubusercontent.com/88386173/162728127-cde5776b-6562-4dc9-bf71-4ea8d56dbf7f.JPG" />
</p>
 
## StartButton
 
 <p align="center">
  <img width="250" alt="StartButton" src="https://user-images.githubusercontent.com/88386173/162729189-d608f3d3-5bf5-4a63-9f88-00e8baacdbd5.png" />
</p>
 
<p align="center">
<img width="650" alt="Allgemein" src="https://user-images.githubusercontent.com/88386173/162728603-93c935e9-357f-4ac7-ae9f-8a6b1e66261c.JPG" />
</p>

 <p align="center">
<img width="650" alt="addSpritze" src="https://user-images.githubusercontent.com/88386173/162728649-34611d5d-e4c5-4d5a-98a1-9f7fe8ed0293.JPG" />
</p>
 
 
## Spritze
 
<p align="center">
<img width="100" alt="Spritze" src="https://user-images.githubusercontent.com/88386173/162729308-170eebfc-4aba-4785-bd43-c1c5957426f7.png" />
</p>

<p align="center">
<img width="650" alt="Spritzeallg" src="https://user-images.githubusercontent.com/88386173/162728781-a29b4f3b-1a1a-412e-8d49-069831d6b69e.JPG" />
</p>

<p align="center">
<img width="650" alt="moveanddropp" src="https://user-images.githubusercontent.com/88386173/162728846-f801087a-aa51-461c-adfd-c72116d75541.JPG" />
</p>

## Antikörper
  
Der Antikörper wird auf dem Start-Screen in die Welt gesetzt.

<p align="center">
  <img width="250" alt="Antikörper" src="https://user-images.githubusercontent.com/88386173/152698020-950b4e70-1960-4ee4-9d61-b14cc83ca149.PNG" />
</p>

 <p align="center">
  <img width="900" alt="Antikörperallg." src="https://user-images.githubusercontent.com/88386173/162726009-0193f275-3641-49d9-b691-40447fdd1079.JPG" />
</p>
 
 <p align="center">
  <img width="900" alt="Fortbewegung" src="https://user-images.githubusercontent.com/88386173/162726225-5b13261f-197d-45e3-b724-3164b9a2b5fb.JPG" />
</p>

 <p align="center">
  <img width="900" alt="kill" src="https://user-images.githubusercontent.com/88386173/162726318-09ad2d34-5cd4-4f6a-83b4-c67b8fb8f187.JPG" />
</p>

 <p align="center">
  <img width="900" alt="eaten" src="https://user-images.githubusercontent.com/88386173/162726410-64c3f71a-d78e-4b15-9e64-37190a50470c.JPG" />
</p>

## Corona Virus

<p align="center">
<img width="259" alt="Virus" src="https://user-images.githubusercontent.com/88386173/152698129-0ca5576c-3438-45a8-adbd-3b08ba420612.PNG" />
</p>
  
<p align="center">
<img width="259" alt="virus traurig" src="https://user-images.githubusercontent.com/88386173/152698284-aac60cfd-7d98-4179-b87f-f393aabc0e62.PNG" />
</p>
 
 <p align="center">
  <img width="650" alt="move" src="https://user-images.githubusercontent.com/88386173/162728278-a9d22436-9dda-43d9-9994-2abd151c9ef2.JPG" />
</p>
 
## Alu (Aluhut)
 
<p align="center">
<img width="100" alt="Actors" src="https://user-images.githubusercontent.com/88386173/162729778-18bc58ad-b345-45a7-9cac-de03c0118236.png" />
 </p>

<p align="center">
<img width="650" alt="Aluallg" src="https://user-images.githubusercontent.com/88386173/162729448-56552ad7-86e4-4e25-9665-689ef1c2fd3f.JPG" />
</p>

<p align="center">
<img width="650" alt="appear" src="https://user-images.githubusercontent.com/88386173/162729543-1fb8e665-f79d-409a-8996-45a87ec24484.JPG" />
</p>

<p align="center">
<img width="650" alt="kill" src="https://user-images.githubusercontent.com/88386173/162729594-82c28171-8d23-4b07-bfae-c5d9e8397417.JPG" />
</p>
 
<p align="center">
<img width="650" alt="disappear" src="https://user-images.githubusercontent.com/88386173/162729641-1f1ccb19-6420-4abe-aab6-3bbf1df96600.JPG" />
</p> 

## Shooter
 
<p align="center">
  <img width="100" alt="Shooter" src="https://user-images.githubusercontent.com/88386173/162730377-50c6d2fa-2108-4be2-b434-748d4752e4eb.png" />
</p>

<p align="center">
<img width="700" alt="Allg" src="https://user-images.githubusercontent.com/88386173/162730321-632c9d41-f98b-4c9e-ba19-a2127b3530af.JPG" />
</p>

## Shot
 
<p align="center">
<img width="50" alt="Shot" src="https://user-images.githubusercontent.com/88386173/162730430-6f50961d-f09c-4be3-8279-b43d929504e8.png" />
</p>

<p align="center">
<img width="750" alt="Allg" src="https://user-images.githubusercontent.com/88386173/162730601-2a1c4f6a-edb5-4150-8d68-1899c94d949a.JPG" />
</p>

<p align="center">
<img width="750" alt="delete" src="https://user-images.githubusercontent.com/88386173/162730641-fc378b4b-c9d7-40e4-8fd8-5ef08f9318ae.JPG" />
</p>

<p align="center">
<img width="750" alt="mover" src="https://user-images.githubusercontent.com/88386173/162730693-9272250f-c732-4c3b-b3cf-a0dc409be736.JPG" />
</p>

## NewGame
 
<p align="center">
<img width="100" alt="PlayAgain" src="https://user-images.githubusercontent.com/88386173/162730888-746e34e3-d882-4ffb-90f6-2a97e0a4296b.png" />
</p>
 
<p align="center">
<img width="750" alt="AllgPlayAgain" src="https://user-images.githubusercontent.com/88386173/162730830-23d5e9da-3bfb-4855-9cc8-1ed96677b7de.JPG" />
</p>


</details>

<details>
<summary>Sounds</summary>
<br>
Dies sind unsere Sounds...
 
</details>

### <a name="2"></a>Blog

<details>
<summary>Der Blog</summary>
<br>
  
## 21-12-2021
Unsere Gruppe hat heute angefangen, über neue Projekt Ideen nachzudenken. Anschließend haben wir recherchiert, welche Programme und Programmiersprachen für Anfänger geeignet sind. Dies war etwas schwierig, einfach wegen der Fülle an Auswahlmöglichkeiten, die online vorhandens sind. Mit Hilfe einer Beratung von Herrn Buhl haben wir uns dazu entschlossen, ein neues Coding Programm auszuprobieren und nicht mehr in Blocksprache zu coden, sondern uns an das "echte" Coden zu wagen. Schnell sind wir zu Greenfoot gelangt, ein für Ausbildungszwecke entwickeltes Programm, bei welchem man mit Java programmiert. Herr Buhl hat uns einen großen Teil der Stunde, die Basics von Greenfoot mit "Actors" und "Worlds" erklärt und wie diese miteinander interagieren und man programmiert.

## 22-12-2021
Wir haben uns erste Spiele bei Greenfoot angeschaut, wie ein Raketenspiel, um das Prinzip dahinter besser zu verstehen.

## 11-01-2022

Heute hat sich Vanessa weiter mit Greenfoot beschäftigt. Nun wissen wir etwas mehr über Greenfoot und was / wieviel wir damit programmieren können. Wir überlegen weiterhin, was wir konkret mit Greenfoot machen wollen, weswegen wir uns weiterhin über dieses Programmier-Portal informiert haben und verschiedene Dinge damit ausprobiert haben. Nun wissen wir, wie wir die Actors zum Bewegen bekommen. Das Kommando move(50) lässt den Actor automatisch nach rechts bewegen, wenn der "Run" Button berührt wird, genau so wie TurnTowards(), wodurch er sich eine eine andere Richtung (hin zu etwas) bewegt. Auch wenn das schon eine erste Erkenntnis ist, müssen wir natürlich noch daran arbeit. Am Ende soll es nämlich ein Spiel werden, was mit den Tasten der Tastatur spielen kann und nicht eine Simulation. Dafür hat uns Herr Buhl auch ein Buch gegeben, mit einer Einführung zu Greenfoot. Dieses hat Vanessa dann mit nach Hause genommen.

Erster Fortschritt:

![cakecode](https://user-images.githubusercontent.com/88386321/149143439-dc78d9d9-21ff-4080-a3c1-d8c94151a41a.PNG)
![mousecode](https://user-images.githubusercontent.com/88386321/149143135-7704f5c2-0cdf-4ff8-878f-937b58a161c5.PNG)
  
Erster Codes für zwei sich bewegende Objekte (Actors).

![restingactors](https://user-images.githubusercontent.com/88386321/149143188-e60a1076-9b70-44f7-af10-342fa5b1708d.PNG)
  
Objekte (Actors) in der Welt.

![runningactors](https://user-images.githubusercontent.com/88386321/149143281-abfe9a30-c43e-4e4d-95e9-94397fa81a41.PNG)
  
Die Objekte nachdem "Run" gedrückt wird. 

## 12-01-2022

Heute hat die Stunde etwas später begonnen (ca. 13:20). Da wir nicht so viel Zeit hatten, haben wir uns mit dem Buch beschäftigt, was uns Herrn Buhl am Tag zuvor gegeben hat, um Java und Greenfoot nach wie vor besser nachzuvollziehen. Schliesslich hat Vanessa angefangen, den vorgegebenen Tutorials folgend etwas neues auf Greenfoot zu programmieren. 
 
## 18-01-2022
Was haben wir gemacht?
  
## 19-01-2022
Wir haben eine Mindmap mit unseren Finalen Ideen für unser neues Projekt erstellt:

<p align="center">  
<img width="1010" alt="Informatik12 2" src="https://user-images.githubusercontent.com/88386173/152692115-733754d4-b3d2-42aa-a9e8-5ea66cd2479d.PNG" />
</p>
  
1. Idee: Ein Klavier programmieren, bei dem Töne erscheinen, wenn man verschiedene Tasten drückt. Zusätzlich kann man seine Werke aufnehmen und immer wieder abspielen, oder sogar die Art von Tönen verändern, wie in eine Orgel. 
2. Idee: Ein Spiel, in welchem man ein Antikörper ist, der einen Coronavirus jagt. Es spielt sich in einer Ader ab und das Ziel ist es, den Virus zu fangen. Dabei treten Hindernisse auf, wie statische Aluhüte, denen man ausweichen muss, oder Globulis, die auf einen geschossen werden. Wenn man eines von beiden berührt ist das Spiel vorbei.
  
Wir haben uns darauf geeinigt, die 2. Spielidee zu verwirklichen und sammeln nun Codes, die wir benötigen.
  
## 25-01-2022
Ausgefallen  

## 26-01-2022
Ausgefallen

## 01-02-2022
Vanessa hat angefangen das Spiel zu programmieren. Nachdem sie das Greenfoot Buch zum grössten Teil durchgelesen hat und Zuhause Videos zum Programm geschaut hat, hat sie probiert, ein "Test-Spiel" mit ähnlichen Funktionen zum geplanten Endspiel zu erstellen. Zunächst hat sie die drei Actors "pizza", "leaf" und "shots" in die Welt gesetzt. Dabei soll "pizza" das "Antikörper" darstellen und "leaf" das "Coronavirus". Das Spiel sollte demnach daraus bestehen, dass das Antikörper probiert, den sich durchgehend bewegenden "Virus" abzuschießen. Der erste Schritt war also, dass "pizza" den Actor "shots" beim drücken der Leertaste auf "leaf" schiesst. Dabei soll sich Pizza später auch noch nach oben und nach unten bewegen können. Die Funktion des Abschießens wurde diese Stunde programmiert:
  
![game(1)](https://user-images.githubusercontent.com/88386321/154082477-b08c25bf-9796-41f2-98ac-1d65115aed51.PNG)
  
Screen mit den Actors "pizza" und "leaf"
  
![game(2)](https://user-images.githubusercontent.com/88386321/154082674-6b0cf9e6-8f13-4abf-8ee1-a685c39c30a3.PNG)
  
Screen, nachdem "shots" durch drücken der Leertaste geschossen wurde

Codes zum abschiessen von "shots":

![pizzacodes](https://user-images.githubusercontent.com/88386321/154083433-de33620e-d32b-4065-b185-f1709b1e6196.PNG)


## 02-02-2022
  
## 08-02-2022
Antonia hat zuhause, da sie krank war und in ein paar Stunden gefehlt hat, weiter gearbeitet. Zum einen hat sie Github aktualisiert und den Aufbau der Seite weiter ausgearbeitet. Dann hat sie im Greenfoot Buch erste Codes herausgesucht, die für unser Spiel nützlich sein könnten. Zuletzt hat sie unseren Spiel Hintergrund und die Charaktere gezeichnet, sodass wir diese ins Spiel einarbeiten können.
Farhat hat zuhause, da sie krank war, für Antonia und Vanessa mögliche Codes recherchiert für die Art von Spiel, die wir umsetzen wollen.
In der Stunde haben wir angefangen eine zweite Version von unserem Spiel zu programmieren. Der Unterschied zur anderen Version liegt dabei, dass sich der Protagonist nicht vor und zurückbewegt, sondern er sich ständig fortbewegt und man mit den links und rechts Tasten  nur der Winkel ändern kann. Zusätzlich zu der Steuerung haben wir auch schon den Antagonisten erstellt, welcher, wenn der Protagonist ihn berührt, verschwindet. Der Antagonist bewegt sich von alleine und völlig zufällig fortwärts und dreht um, wenn er den Bildschirmrand berührt. 
Bisher sind unsere actors nur durch "Platzsteller" besetzt, da die Bilder, die Antonia zuhause erstellt hat momentan noch nicht funktionieren. Sie haben, obwohl sie freigestellt sind, immer noch einen weißen Rand und erscheinend viel zu groß. Dieses Problem wollen wir noch lösen. 
  
<p align="center">
<img width="900" alt="code world" src="https://user-images.githubusercontent.com/88386173/153778984-662cd5d7-3dc2-49ce-9715-49a6f12ccd18.png" />
</p>
  
Das hier ist die Code Übersicht unserer World, in der das eigentliche Spiel stattfindet. Hier werden die beiden Charaktere Corona und Antikörper zu Anfang des Spiels hinzugefügt. 
  
<p align="center">
<img width="900" alt="code antigen" src="https://user-images.githubusercontent.com/88386173/153778772-71122d78-4177-434e-9893-a7079ab405be.png" />
</p>
  
 Der obere Code bewirkt, dass sich der Protagonist bei rechter/linker Pfeiltaste jeweils um 3 Grad dreht. 
 Der untere Code bewirkt, dass  der Protagonist bei Berührung den Antagonist ("Corona") "isst", dieser also verschwindet.
 
 <p align="center">
<img width="900" alt="code corona" src="https://user-images.githubusercontent.com/88386173/153778885-a0d5b124-b583-4562-89bb-ec2eebcdf022.png" />
</p>

Dies sind die ersten Codes des Antagonisten "Corona". Der obere code ist dafür da, dass sich Corona fortbewegt und dabei sich in zufällig erstellten Winkeln dreht um die Richtung zu wechseln.
Die beiden unteren Codes beschreiben, wie zuvor erwähnt, dass  Corona, falls es den Rand berührt, abprallt und in die genau andere Richtung (180 Grad) weiter bewegt.
  
<p align="center">
<img width="400" alt="world 1" src="https://user-images.githubusercontent.com/88386173/153779031-397eeaa0-ba1c-4ec3-8e6c-d07114397cb1.png" />
</p>
  
Und hier sieht man nun final unseren ersten Entwurf des Spieles. Das Mader-ähnliche Tier stellt den Gegner da, das K steuert der Spieler. Wichtig zu erwähnen ist hier, das alles, sowohl die Kostüme der actors als auch der Hintergrund bisher nur Platzhalter sind und sich noch ändern sollen.
  
Zusatz: Da Vanessa und Antonia  sich falsch verstanden haben und an zwei verschiedenen "Arten" des Spiels gearbeitet haben (vgl 08.02.2022), mussten wir sämtliche Codes, die Vanessa eigentlich programmiert hatte, verwerfen.
  
Vanessa hat also Plan geändert und die Rollen von "pizza" und "leaf" umgedreht. "Pizza" soll nun das Antikörper sein, welches vom Actor "leaf", unserem Aluhüttchen, abgeschossen werden soll. Die Funktionen, des sich Hoch- und Runterbewegens waren also nicht mehr nötig, genauso wie das weitere Programmieren des sich automatisch Hoch- und Runterbewegenden "leaf"-Actor. Nachdem Antonia und Vanessa das Missverständnis geklärt haben und sich dazu entschieden haben, an Antonias "Jagd"-Version weiter zu codieren, hat sich Vanessa mit unterschiedlichen Codes auseinander gesetzt, die man in die richtige Version einsetzen könnte. Der nächste Schritt war für sie, ein Code zu finden, durch welchen der Actor "pizza" verschwindet, sobald er vom abgeschossenen Actor "Shots" berührt wird. 
  
Code für das Verschwinden von "pizza" nach dem Abschießen von "Shots":
  
![shotnewcode](https://user-images.githubusercontent.com/88386321/157477273-3c111640-72f4-4b73-8a77-35ed253a602f.jpeg)


## 09-02-2022
Vanessa und Antonia haben sich aufgeteilt und coden jeweils beide an einer der beiden App-Versionen weiter. Am Ende wollen wir dann die Funktionen, die uns am besten gefallen, zu einem Spiel zusammensetzen. 
So hat Vanessa weiter an einer "Schieß-Funktion" gecodet, die wir später für Hindernisse nutzen wollen, die auf unseren Protagonisten schießen, oder er kann auf diese schießen.
Antonia hat währenddessen eine zweite subworld erstellt und auf dieser einen Startbutton-actor eingeführt, bei welchem auf Knopfdruck das Spiel startet. Da Greenfoot andauernd abgestürzt ist, konnte sie ihn bisher nicht testen und muss dies nächste Stunde tun. Zuhause hat Antonia den GitHub für die letzten Tage geupdatet.

## 15-02-2022
Antonia hat einen Start Screen als neue World eingefügt, die als erstes erscheint, wenn man das Spiel startet. Darauf ist ein Actor mittig platziert, welcher wie ein Startknopf aussieht. Wenn man auf "Button" drückt, erscheint der Gaming Screen und der Coronavirus fängt schon an sich zu bewegen. 
Den Actor, den der Spieler selbst steuert, das Antikörper, fängt erst an sich zu bewegen, wenn man die Eingabetaste klickt. Dies haben wir mit einer Boolean Funktion codiert, die immer false ist, außer wenn die Eingabetaste gedrückt wird. Und die Aktionen des Antikörper arbeiten nur, wenn Boolean true ist. 
Nachdem dies eingestellt war, hat sich Antonia an die Einführung eines Hindernis promiert. Wir wollten Querdenker, sogenannte "Alu"s (wegen Aluhüte), die immer wieder random auftauchen und nach ein paar Sekunden wieder verschwinden. Wenn das Antikörper gegen einen Alu stößt, ist das Spiel verloren.
Der Code sieht vor, dass  der Computer eine Zahl zwischen 0 und x random generieren soll. Ist diese Zahl 15, wird ein Alu an eine beliebige Stelle im Spiel platziert. Allerdings hat sie dazu noch nicht die Funktion erstellt, dass Alu nach ein paar Sekunden wieder verschwindet, weshalb sie in der Test- und Suchphase nach einer passenden Zahl, von Alus überschwemmt wurde. Doch nach ein paar Versuchen, hat sie eine gute Zahl gefunden, wo Alus in einem angemessenen Abstand spawnen.
  
<p align="center">
<img width="700" alt="startbutton" src="https://user-images.githubusercontent.com/88386173/156214139-04980902-3b87-42fd-bec8-1a2497f6e4b9.PNG" />
</p>
Dies ist der StartButton, der das Spiel startet.
  
  <p align="center">
<img width="700" alt="gegner" src="https://user-images.githubusercontent.com/88386173/156213672-2d6295b6-b3cb-4e48-82a2-829dd9057b8e.PNG" />
</p>
  
Dies ist der Code, damit Gegner nach einer zufälligen Zeit auftauchen und das Spiel verloren ist, wenn das Antikörper Alu berührt.

Vanessa hat sich mit der Frage beschäftigt, wie die Shots, nachdem sie geschossen wurden, verschwinden können. Nach dem Abschießen bliben diese natürlich am Rand des Spiels hängen, was ja im wahren Spielen vermieden werden sollte. Sie hat sich also im Forum und in der Greenfoot-Bibliothek über mögliche Codes informiert und auch verschiedene ausprobiert. Jedoch hat keiner von diesen funktioniert. Ihre Aufgabe war es also, nach einem passenden Code zu suchen. Weiter beschäftigt sich Vanessa auch mit der Frage, wie "Shots" automatisch geschossen werden kann, da diese Funktion zu einem Actor gehört, den wir nicht kontrollieren sollen, sondern der den Spieler in verschiedenen Zeitabständen abschießen soll.
  
## 16-02-2022
Antonia hat heute den Start-Button auf dem Startscreen resized, da dieser viel zu groß war. Dazu hat sie die beiden End-Screens loose and win provisorisch erstellt und ins Spiel eingebettet. Bis zur nächsten Stunde will sie die endgültigen Screens für das Ende designen.   
Farhat war heute auch wieder da und schaut uns über die Schulter. Zusätzlich probiert sie sich selbst im programmieren und recherchiert im Internet nach nützlichen Codes.
  
<p align="center">
<img width="500" alt="startbuttonsize" src="https://user-images.githubusercontent.com/88386173/156215523-88df1fe1-7f48-4fac-b59a-f9c46c3ac9d1.PNG" />
</p> 
Dieser Code passt die Größe des Buttons an.
  
Vanessa hat zusammen mit Herrn Buhl den richtigen Code zum Verschwinden von "Shots" am Rand gefunden und diesem im Spiel eingebaut (einen Code, den sie unter anderem schon probiert hatte, jedoch falsch programmiert hatte). Außerdem hat sie eine Lösung gefunden, wodurch "Shots" in bestimmten Zeitabständen vom Actor "leaf" geschossen werden kann. Diesen Code plant sie nächste Stunde zu programmieren.
  
![shotnewcode](https://user-images.githubusercontent.com/88386321/157490166-a99244e7-9ea2-4947-a0ad-9d43e904a691.jpeg)

Code der "Shots"-Klasse zum Verschwinden 
  
## 22-02-2022
Antonia hat bei den Alus (die Hindernisse) nun versucht einen Timer einzuführen. Wenn dieser abgelaufen ist, soll das spezifische Alu wieder verschwinden. Allerdings scheint irgendwo im Code ein Fehler zu liegen, den sie partout nicht finden kann. Denn anstatt nach einigen Sekunden zu veschwinden, verschwindet Alu sofort und taucht auch nie wieder auf. Da sie den Fehler im Code vorerst nicht finden kann, macht sie erstmal was anderes. Sie führt die endgültigen Loose- and Win-Screens ein. Dazu ändert sie vom Antikörper das provisorische Kostüm (ein roter Kreis mit "K" drin) zu dem endgültigen Kostüm, dass sie extra zuhause gezeichnet hat.

Vanessa hat hingegen die Funktion zum automatischen Schießen von "Shots" codiert. Dafür hat sie in der Bowser-Klasse von "leaf" die Maximale und Minimale Verzögerung zwischen den Schüssen angegeben, wobei sie die Parameter 40 und 160 gewählt hat. Der Timer, welche die Funktion "shoot()" der "leaf" Klasse aufruft, besteht aus der Summe von dem Minimalwert (40) und eine willkürliche Zahl zwischen den Parametern, wobei diese Funktion wiederholt läuft.
  
![leafcodenew](https://user-images.githubusercontent.com/88386321/157482899-57747368-0619-40a3-b1b0-5dbda127a2e0.PNG)

Erste Code: Timer der "Shots"
  
## 23-02-2022
Herr Buhl hat Vanessa und Antonia eine weitere, ausführlichere Ausführung in Greenfoot gegeben und ihnen weitere Codes und Möglichkeiten präsentiert. Auch hat er den Fehler in Antonias Alu-Timer gefunden (ein ";", wo es nicht hingehörte). Der Code funktioniert nun also.
  
<p align="center">
<img width="700" alt="timer" src="https://user-images.githubusercontent.com/88386173/156214506-92c66ef4-94ee-4874-b7e4-75f6f6990f08.PNG" />
</p>
  
Das fehlerhafte Simokolon kann man in der if Funktion sehen. Ohne dieses funktioniert der Code.
  
Herrn Buhl konnte Vanessa mit dem Problem der willkürlichen Schüsse helfen. Da "Shots" nicht nur horizontal und in eine Richtung geschossen werden sollte, sondern in mehreren Richtungen, bedarft es auch einen entsprechenden Code. Vanessa hatte zunächt mit der Funktion Greenfoot.getRandomNumber einen Code zu erstellen, durch welchen eine willkürliche Nummer ausgesucht werden solle, die durch andere Codes eine Schussrichtung angeben sollte. Dies hatte leider nicht funktioniert. Dennoch konnte Herrn Buhl uns dabei helfen, einen anderen Code zu finden.
  
![shotnewcode](https://user-images.githubusercontent.com/88386321/157486181-e1497787-44db-4ec1-b6de-a205c3cb10f4.PNG)

Der Code gehört zur "Shots"-Klasse. Der obere Teil in der Bowser-Klasse gehört zur Ausführung der Funktion. Der Code der "leaf"-Klasse ruft die Funktion für den Actor "Shots" auf.
  
![leafcodenew](https://user-images.githubusercontent.com/88386321/157486779-1d5f9549-15e1-44bd-8907-e5eade30cbbb.PNG)

Der zweite Code gehört zu "leaf" und basiert auf dem schon erahnten Prinzip von "Greenfoot.getRandomNumber". Er dient zur willkürlichen Schieß-Funktion von "leaf"

  
## 01-03-2022
Antonia hat zuhause den GitHub aktualisiert und die Sachen eingetragen, die sie in den letzten 2 Wochen programmiert hat. Sie hat auch einen neuen Start-Screen designt. Im Unterricht hat sie dann direkt den neuen Start-Screen eingeführt. Dann hat sie eine kleine Animation programmiert, die abläuft, nachdem man den StartButton gedrückt hat (dieser verschwindet dann). Eine Spritze erscheint im Bild und bewegt sich nach links. An einer bestimmten Koordinate (X/Y), setzt sie ein Antikörper in die Welt (der Körper ist nun geimpft). Die Spritze bewegt sich weiter, bis sie den linken Rand berührt, dann öffnet sich das eigentliche Spiel. Nachdem dies funktioniert hat, hat sie das provisorische Corona Kostüm gegen das Echte ausgetauscht. Danach wurden alle Actors so unbenannt, dass sie am Anfang großgeschrieben werden und dementsprechend die Codes noch überarbeitet.
Farhat hat als erstes nach einem Bild für unseren Alu-Actor gesucht. Danach hat sie auch gecodet. Sie hat ausprobiert, wie man Soundeffekte bei bestimmten Interaktionen und allgemein eine Melodie im Hintergrund einrichten kann. Dies wollen wir, wenn die Zeit es zulässt, noch auf unser Spiel übertragen.
Zum Schluss der Stunde hat Vanessa das Erste Mal probiert, die seperat programmierten Codes zusammenzufügen. Dies heißt konkret, dass wir Alu nun auch schießen lassen wollen. Die Codes an sich haben keine Fehler, aber sie funktionieren zusammen nicht so gut, wie einzeln. Wir werden nun versuchen den Fehler zu finden. Sonst haben wir die Idee, das wir 1 statischen Alu zusätzlich einführen, der immer da ist, und als einziger schießt. An diese Funktion soll nun Vanessa arbeiten.

<p align="center">
<img width="500" alt="neuerbutton" src="https://user-images.githubusercontent.com/88386173/156214849-93ae399c-836e-4dd4-a684-2fcf001d4ec2.PNG" />
</p> 
  
Der StartButton wurde für die Animation am Anfang umfunktioniert. Wenn dieser geklickt wird erscheint nun nicht direkt die Game-World, sondern der Knopf verschwindet und eine Spritze erscheint. 
 
<p align="center">
<img width="700" alt="Spritzecode" src="https://user-images.githubusercontent.com/88386173/156215546-19f20811-6cd7-43c5-9f5f-dd658dcce9c3.PNG" />
</p> 
  
Dies ist der Code für den neuen Actor "Spritze". Die Spritze bewegt sich nach links (also auf der X-Achse immer minus 1) und auf dem Weg setzt sie bei 200/200 ein Antikörper ab, der Körper ist nun also "geimpft". Wenn sie den Rand berührt (ifAtEdge), wird das eigentliche Spiel gestartet.

## 02-03-2022
Da wir mit der Entwicklung des Spiels schon ziemlich weit sind und planen, in der nächsten Doppelstunde den Fehler der Alus zu beheben, haben sich Antonia und Vanessa zusammengesetzt um weitere Ideen für das Spiel zu konzipieren. Sie sind zu dem Entschluss gekommen, dass sie den von Farhat gesuchten Code für Soundeffekte einbauen wollen und auch an eine Funktion arbeiten wollen, die Schriftzüge (z.B. Hilfe, rette mich vor Corona!) einblenden lässt. Letztere Fuktion wird sich Antonia widmen während Vanessa probiert den Fehler zu beheben. Außerdem hat Vanessa diese Stunde sämtliche Screenshots von Codes gemacht und einige alte Codes nachgestellt, die sie vergessen hatte, zu screenshoten.
 
## 08-03-2022
Heute ist der Unterricht wegen eines Ausfluges ausgefallen.
  
## 09-03-2022
Heute hat sich Vanessa weiterhin mit dem Problem der Aluhütte beschäftigt. Die verschiedenen Codes hat sie alle abgeglichen und verschiedene Fehler (Falsche Benennung der Actors) korrigiert. Es scheint jedoch, dass es immmer noch zu Fehler kommt, weswegen wir nun beschlossen haben, zwei verschiedene (Alu-)Actors zu erstellen, von denen einer die programmierte Schießfunktion besitzt und der andere willkürlich, als Hinderniss, spawnt. Außerdem hat Vanessa Zuhause ihre fehlende Einträge nachgetragen und den Github vervollständigt.   
Antonia hat versucht, einen Code zu programmieren, um einen bestimmten Text am Anfang des Spieles erscheinen zu lassen. Nebenbei hat sie Farhat dabei unterstützt, Codes auszuprobieren, die Soundeffekte oder Hintergrundmelodien erscheinen lassen.

## 15.03.2022
Antonia hat zu Anfang der Stunde die Lösung für den Text gefunden und ihn auch in das Spiel eingebaut.
Vanessa hat währendessen dass Zusammenführen beider Versionen des Spiels, die wir programmiert haben, wiederholt, da beim ersten Mal irgendwo ein Fehler geschehen ist. Am Ende haben wir alle am Spiel gearbeitet und die Funktionen aller Actors geprüft. Dass Zusammenführen der Codes hat geklappt und die Roh-Version unseres Spieles funktioniert.
 
## 16.03.2022

 
## 22.03.2022
Wir wollen einen Text als Anleitung (Zum Beispiel "Steuer mit den Pfeiltasten" am Anfang des GameScreens erscheinen lassen. Dieser soll aber auch wieder verschwinden (zum Beispiel wenn man enter drückt, oder nach einer bestimmten Zeit). Wir haben sowohl eine if (-else) Funktion, als auch mit Boolean ausprobiert, doch dies führte beides nicht zu dem gewünschten Ergebnis. Unser Fehler war, dass wir dachten, dass wenn bei Boolean/if das andere erfüllt wird, dass Erste dann verschwindet. Doch so ist es nicht. Wir hätten zwar auch mit einem Image arbeiten können, haben uns aber dagegen entschieden und stattdessen den Text auf den StartScreen gepackt. Dort verschwindet er automatisch, sobald ein neuer Screen (Game Screen) geöffnet wird.
 
<p align="center">
<img width="600" alt="text" src="https://user-images.githubusercontent.com/88386173/162736254-b51afb5b-9ebd-4776-b821-97e41edf1f39.JPG" />
</p>

## 23.03.2022
Frei wegen der mündlichen Englisch Prüfungen
 
## 29.03.2022
Letzte Informatikstunde. Vanessa und Antonia haben beide Corona. Farhat ist krank.
 
## 06.04.2022
Herr Buhl ist netterweise in die Schule gekommen. Somit konnten Vanessa und ich das Spiel einmal so abspeichern, so dass wir auch von zuhause weiterarbeiten können. Außerdem hat auch er nochmal über unsere Codes geschaut und uns geholfen. So hat er uns in der Annahme bestätigt, dass wir das vorherige Textproblem wahrscheinlich nur mit einem Image lösen hätten können. 

## Osterferien
Wir haben die Sounds in das Spiel integriert. So gibt es jetzt ab dem Game Screen eine durchgehende Melodie im Hintergrund. Zusätzlich gibt es Klick-Geräusche, wenn man einen Knopf drückt und einen Applaus oder eine traurige Melodie, je nachdem ob man verliert oder gewinnt.
Auch haben wir einen PlayAgainButton etabliert. Dieser erscheint auf dem Win- oder LooseScreen und ermöglicht ein schnelles Neustarten des Spieles. Da sich dabei aber die Hintergrundmusik selbst übereinandergelegt hat, mussten wir diese statisch codieren (Siehe Bild unten). Nun bleibt die Musik ab Spielbeginn durchgehend erhalten und startet nicht jedes mal neu und überlagert sich dadurch selbst.
 
<p align="center">
<img width="600" alt="Static" src="https://user-images.githubusercontent.com/88386173/162736069-67aeada5-9358-43c8-be22-8be42da43765.JPG" />
</p>
 
Weiterhin haben wir, nachdem das Spiel fertig gestellt war, Screenshots von allen Codes erstellt und in Github eingearbeitet. Danach haben wir die Codes erklärt und das Fazit geschrieben.

</details>
  

### <a name="3"></a>Fazit

### <a name="4"></a>Finale Links

Notizen:
<p align="center">
<img width="250" alt="Actors" src="" />
</p>



