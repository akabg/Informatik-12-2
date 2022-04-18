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
Die Idee des Spiels ist es, dass der Spieler einen Antikörper steuert. Dabei muss er mithilfe der Pfeiltasten ein Coronavirus jagen. Wenn der Antikörper das Virus berührt, hat der Spieler gewonnen. Um die Schwierigkeit zu erhöhen, gibt es auch Hindernisse, die Aluhüte, denen man ausweichen muss, oder die auf einen schießen. Letztendlich hat man auch nur eine bestimmte Zeit zum Einfangen, da ein Timer runterläuft.
Programmiert haben wir mit Greenfoot, eine interaktive Java-Entwicklungsumgebung. Dies war für alle in der Gruppe das erste "echte" programmieren.
Der Look und auch das Prinzip des Spieles sollen  an ein 90er-Jahre Arcade Spiel erinnern. Manche der Actors haben wir selbst gezeichnet, so wie den Antikörper, Corona und auch die Aluhüte. Auch die Loose- und Win-Screens haben wir selbst designt. 
Die Idee für das Spiel kam einfach aus der damaligen Corona-Situation heraus. Wir wollten das Thema der Querdenker (Aluhüte), dem Impfen und natürlich dem Coronavirus selbst humoristisch aufarbeiten, um auch einfach mal darüber lachen zu können.
</details>


<details>
<summary>Aufbau</summary>
<br>

### 1. Start Screen
Wenn man das Spiel startet, trifft man als erste auf den StartScreen. Wenn man den StartButton drückt, verschwindet er und stattdessen wird eine Spritze in die Welt gesetzt, die die Impfung darstellen soll. Zusätzlich wird der Schriftzug "Hilfe, rette mich vor Corona!", "Drücke gleich enter zum Starten." und "Steuere den Antikörper mit den Pfeiltasten" angezeigt. Dies sind alle Anweisungen, die der Spieler an die Hand bekommt.
Die Spritze bewegt sich über den Bildschirm nach links und setzt auf halben Wege ein Antikörper (den der Spieler später steuert) in die Welt. Wenn die Spritze den Rand des Screens berührt, wird der GameScreen geöffnet.
 
### 2. Game Screen
Hier beginnt das eigentliche Spiel. Das zu fangende Objekt, Corona, fängt sofort an sich zufällig über den Bildschirm zu bewegen. Der zu steuernde Antikörper fängt erst an sich zu bewegen und sich steuern zu lassen, wenn man die Eingabetaste drückt. Die Aluhüte lassen sich unterscheiden in einen, der statisch ist und mit Bällen zufällig um sich schießt und Aluhüte, die direkt zufällig spawnen und nach kurzer Zeit wieder verschwinden. Wenn man einen Aluhut berührt, oder man von einem Ball abgeschossen wird, hat man verloren. 
Man spielt also klassisch das Spiel und versucht dabei nicht zu sterben und im Rahmen der Zeit das Coronavirus zu fangen. Während des Spiels läuft im Hintergrund durchgehend eine Melodie. Am Ende des Spiels öffnet sich, je nach Ausgang, entweder der Win-Screen oder der Loose-Screen.

### 3.1 Win-Screen
Man gewinnt, wenn der Antikörper Corona berührt. Dann öffnet sich der Win-Screen und ein Applaus ertönt. Zusätzlich hat man hier die Option auf einen 'Play Again' Button zu drücken, um direkt wieder zu dem Game Screen geleitet zu werden.

### 3.2 Loose-Screen
Man landet hier wenn:
- Antikörper Alu berührt
- Antikörper abgeschossen wird
- der Timer abgelaufen ist

 Wenn sich dieser Bildschirm öffnet, ertönt ein trauriger Sound. Auch hier hat man die Option des 'Play Again' Buttons. 
  
</details>

<details>
<summary> World (Setting) </summary>
<br>
 
Es gibt 4 verschiedene Screens/Worlds. Einen StartScreen, ein GameScreen und jeweils ein Loose/Win Screen. Alle spielen in einer Ader, also im menschlichen Blutkreislauf.

### 1. Start Screen
 
Inhalt
- StartButton
- Schriftzüge
- Spritze
- Nicht steuerbarer Antikörper
 
<p align="center">
<img width="600" alt="Start1" src="https://user-images.githubusercontent.com/88386173/162732710-16f9ecd8-2ec9-441d-b9e2-3fdacdb7a9f7.JPG" />
</p>
 
Wenn man das Spiel startet, ist dies der erste Eindruck, den man gewinnt. Wenn man auf den Button drückt, verschwindet dieser und drei Schriftzüge (die Anleitung) und die Spritze werden in die Welt gesetzt. Die Spritze bewegt sich nach links über den Bildschirm und setzt auf dem Weg einen Antikörper in die Welt, der Spieler ist jetzt geimpft (siehe Bild unten). Wenn die Spritze den Rand berührt, wird automatisch der GameScreen geöffnet. Auf dem StartScreen ist außer der StartButton nichts interaktiv. Man kann diesen Teil eher als Animation sehen, die die Geschichte des Spieles darstellt und zusätzlich Zeit gibt, um die Anleitung zu lesen.
 
<p align="center">
<img width="600" alt="Start2" src="https://user-images.githubusercontent.com/88386173/162732774-652f01ce-be59-40f8-bc7e-e4e4ca494a82.JPG" />
</p>
 
<p align="center">
<img width="600" alt="StartCode" src="https://user-images.githubusercontent.com/88386173/162732566-2f1e340e-3cff-49ef-9142-7c3ed5ca5f09.JPG" />
</p>
 
Dies ist der komplette Code des StartScreens. Er ist einfach gehalten, es wird nur der Actor 'StartButton' hinzugefügt, da der restliche Code bei den Actors selbst zu finden ist. 

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
 
Dies ist ein Screenshot, der den Aufbau des Spieles verdeutlicht. Das gelbe Coronavirus bewegt sich sofort selbstständig und zufällig über den Bildschirm. Der Antikörper ist über die Pfeiltasten steuerbar und bewegt sich erst, wenn man die Eingabetaste drückt. Rechts kann man den statischen Aluhut sehen, der Bälle zufällig schießt. Der linke Aluhut ist einer, der zufällig irgendwo spawnt und auch nach kurzer Zeit wieder verschwindet. Es kann auch sein, dass mehrere Aluhüte spawnen. Oben in der Ecke sieht man den Timer, der runterzählt.

<p align="center">
<img width="600" alt="GameCode1" src="https://user-images.githubusercontent.com/88386173/162732820-c555a8bd-6422-485e-84c5-cc7accb92781.JPG" />
</p>
 
Den Code des GameScreens kann man in zwei Teile einteilen. In dem ersten Teil werden alle Actors in die Welt gesetzt. Es wird auch die Geschwindigkeit reguliert. Zusätzlich wird hier für die Hintergrundmusik codiert. Diese ist statisch, da sie sich sonst jedes Mal, wenn man das Spiel neu startet, selbst überlegen würde.
 
<p align="center">
<img width="450" alt="GameCode2" src="https://user-images.githubusercontent.com/88386173/162732826-74bb813f-fe82-4aee-89f5-fb88f6a78226.JPG" />
</p>
 
Der zweite Teil des Codes enthält die Methoden 'countTime' und 'showTime'. 'countTime' zählt den Timer (der auf dem 1. Bild zu sehen ist) runter und öffnet, wenn 0 erreicht ist, denn Loose Screen - man hat verloren. Die 'showTime' Methode zeigt den runterzählenden Timer und davor den Ausdruck 'Timer:' in der linken oberen Ecke im Spiel an, sodass man immer den aktuellen Stand sehen kann. Die restlichen Codes sind auch bei den Actors zu finden.

### 3.1 Win-Screen

Inhalt:
- Play Again Button
 
<p align="center">
<img width="600" alt="WinScreen" src="https://user-images.githubusercontent.com/88386173/162733304-6e2137d5-6c3d-4857-b5af-a16113942233.JPG" />
</p>

Dies ist der Win-Screen, zu welchem man gelangt, wenn man gewonnen hat. Wenn man den 'Play Again' Button drückt, wird man automatisch erneut zu dem GameScreen weitergeleitet.
Der Code (unten zu sehen) ist für den Screen selbst einfach, es wird der Actor 'NewGame' (der 'Play Again' Button) in die Welt gesetzt. 

<p align="center">
<img width="600" alt="WinCode" src="https://user-images.githubusercontent.com/88386173/162733374-dec407f3-642c-4ce3-9b10-353630161b58.JPG" />
</p>

### 3.2 Loose-Screen

Inhalt:
- Play Again Button
 
<p align="center">
<img width="600" alt="LooseScreen" src="https://user-images.githubusercontent.com/88386173/162733471-60b75e3f-29fe-4ffb-afa8-8c5e7f1c7b6e.JPG" />
</p>

Der Loose-Screen ist identisch aufgebaut, wie der Win-Screen.
 
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
 
Dies ist der Actor StartButton, der, wenn man ihn drückt, das Spiel startet. Der obere Code ‚public StartButton‘ setzt das Bild des Actors und verkleinert es um die Hälfte.

 <p align="center">
<img width="650" alt="addSpritze" src="https://user-images.githubusercontent.com/88386173/162728649-34611d5d-e4c5-4d5a-98a1-9f7fe8ed0293.JPG" />
</p>
 
Die Funktion des StartButton ist der public void ‚addSpritze‘.  Dieser wird ausgeführt, wenn man mit der Maus auf den Button klickt. Als erstes wird ein Klick-Geräusch abgespielt. Danach wird der Actor ‚Spritze‘ an einer bestimmten Stelle in die Welt gesetzt und die Anweisungen für den Spieler als Text angezeigt. Zuletzt verschwindet der StartButton.
 
 
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
 
Der Actor ‚Spritze‘ wird über den StartButton in die Welt gesetzt. Die Spritze hat drei verschiedene Funktionen, ‚impfen‘, ‚add‘ und ‚WorldEdge‘. Bei ‚impfen‘ bewegt die Spritze sich nach links über den Bildschirm. Wenn sie die Stelle (250, 100) erreicht, wird ein Antikörper über ‚add‘ in die Welt gesetzt. Dies ist alles eine Animation, die die Impfung nachstellt und genug Zeit gibt, die Anleitung zu lesen. Wenn die Spritze den linken Bildschirmrand erreicht, wird sie durch ‚WorldEdge‘ entfernt und der GameScreen wird geöffnet. 

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
 
Der Antikörper ist der wichtigste Actor in diesem Spiel. Er wird von dem Spieler gesteuert. Wir haben hier mit einer boolean-Funktion gearbeitet, wodurch die startFlag zu Anfang false ist. Dies hat den Sinn, dass die Funktionen des Antikörpers erst funktionieren, wenn man die Eingabetaste drückt und dadurch die startFlag = true ist. Die Funktionen des Antikörpers sind ‚moveandturn‘, ‚eat‘ und ‚eaten‘. ‚Moveandturn‘ ist dafür da, dass man den Antikörper steuern kann. Dieser bewegt sich nur in Kreisbewegungen voran, da man nur mit der linken und rechten Pfeiltaste arbeitet und der Antikörper sich demnach leicht nach links oder rechts rotiert. Wenn man keine Pfeiltaste drückt, bewegt sich der Antikörper vorwärts.

 <p align="center">
  <img width="900" alt="eat" src="https://user-images.githubusercontent.com/88386173/162726318-09ad2d34-5cd4-4f6a-83b4-c67b8fb8f187.JPG" />
</p>
 
Bei ‚eat‘ wurde dafür codiert, dass wenn der Antikörper den Actor Corona berührt, Corona aus der Welt entfernt wird. Außerdem wird ein klatschen-Sound abgespielt und der Win-Screen geöffnet, da man das Spiel gewonnen hat.

<p align="center">
<img width="900" alt="eaten" src="https://user-images.githubusercontent.com/88386173/163677142-9fd5e374-780b-4c55-be8a-1d828b6b08b9.JPG" />
</p>

‚Eaten‘ hingegen sorgt dafür, dass wenn man den Actor ‚Shooter‘ berührt, man auch verloren hat, ergo es wird die traurige Melodie gespielt und der Loose-Screen wird geöffnet.

## Corona Virus

<p align="center">
<img width="259" alt="Virus" src="https://user-images.githubusercontent.com/88386173/152698129-0ca5576c-3438-45a8-adbd-3b08ba420612.PNG" />
</p>
  
 
<p align="center">
<img width="650" alt="move" src="https://user-images.githubusercontent.com/88386173/162728278-a9d22436-9dda-43d9-9994-2abd151c9ef2.JPG" />
</p>
 
Der Actor Corona hat nur eine Aufgabe, nämlich sich willkürlich hin und her zu bewegen.  Mit dem void ‚moveAround‘ bewegt sich das Virus immer vorwärts. Allerdings wird immer wieder eine zufällige Nummer zwischen 0 und 100 generiert Wenn diese kleiner als 10 ist, dreht sich der Actor um einen bestimmten Grad, der auch zufällig generiert wird. Außerdem hat Corona noch die Aufgabe, wenn es einen Rand berührt, sich um 180 Grad zu drehen, sodass es nicht hängen bleibt.
 
## Alu (Aluhut)
 
<p align="center">
<img width="100" alt="Actors" src="https://user-images.githubusercontent.com/88386173/162729778-18bc58ad-b345-45a7-9cac-de03c0118236.png" />
 </p>

<p align="center">
<img width="650" alt="Aluallg" src="https://user-images.githubusercontent.com/88386173/162729448-56552ad7-86e4-4e25-9665-689ef1c2fd3f.JPG" />
</p>
 
Aluhut ist einer der Actor, die der Antikörper nicht berühren darf. ‚Appear‘, ‚kill‘ und ‚disappear‘ sind seine Methoden. 

<p align="center">
<img width="650" alt="appear" src="https://user-images.githubusercontent.com/88386173/162729543-1fb8e665-f79d-409a-8996-45a87ec24484.JPG" />
</p>
 
Bei ‚appear‘ ist dafür codiert, dass eine zufällige Zahl zwischen 0 und 400 generiert wird. Wenn diese Nummer 15 ist, wird ein Aluhut an zufällig generierten Koordinaten in das Spiel gesetzt. So ist gegeben, dass weder das Wo noch das Wann der Aluhüte vorhersehbar ist. 

<p align="center">
<img width="650" alt="kill" src="https://user-images.githubusercontent.com/88386173/162729594-82c28171-8d23-4b07-bfae-c5d9e8397417.JPG" />
</p>
 
Public void kill sorgt dafür, dass wenn der Antikörper einen Aluhut berührt, der Antikörper entfernt, die traurige Melodie abgespielt und der Loose-Screen geöffnet wird. Der Spieler hat verloren.
 
<p align="center">
<img width="650" alt="disappear" src="https://user-images.githubusercontent.com/88386173/162729641-1f1ccb19-6420-4abe-aab6-3bbf1df96600.JPG" />
</p>
 
Allerdings können die Aluhüte auch selber verschwinden. Bei ‚disappear‘ wird ein definierter Timer runtergezählt und wenn er 0 erreicht, wird der Aluhut aus der Welt entfernt. Wenn es dies nicht geben würde, wäre der Screen nach kurzer Zeit voll mit Aluhüten. Außerdem macht es das Spiel spannender, wenn Hindernisse zufällig auftreten und kurz danach wieder verschwinden.

## Shooter
 
<p align="center">
  <img width="100" alt="Shooter" src="https://user-images.githubusercontent.com/88386173/162730377-50c6d2fa-2108-4be2-b434-748d4752e4eb.png" />
</p>

<p align="center">
<img width="700" alt="Allg" src="https://user-images.githubusercontent.com/88386173/162730321-632c9d41-f98b-4c9e-ba19-a2127b3530af.JPG" />
</p>
 
Der Shooter ist ein Aluhut, der sich immer in einer Ecke des Game-Screens befindet und die Fähigkeit besitzt, Globulis, symbolisch dargestllt durch den Actor Shot, durch das Spiel zu schießen. Die Rate der Schussverzögerung, wird durch dem Minimalwert (minShotelay = 40) und dem Maximalwert (maxShotDelay = 160) geregelt. Wenn der codierte shotTimer == 0 entspricht, wird ,shoot' ausgeführt, und zwar in bestimmten Abständen, die von den Schussverzögerungen angegeben werden. Diese Funktion läuft durchgehend. ,shoot' regelt zunächst die Schussausrichtung von Shot, mittels des Greenfoot Ausdrucks ,getRandomNumber(360)', was heißt, dass eine Nummer zwischen 0 und 359 kreiert wird. Shot spawnt somit nach dem Zeit Intervall mit seiner Ausrichtung an der Stelle unseres Shooters. 

## Shot
 
<p align="center">
<img width="50" alt="Shot" src="https://user-images.githubusercontent.com/88386173/162730430-6f50961d-f09c-4be3-8279-b43d929504e8.png" />
</p>

<p align="center">
<img width="750" alt="Allg" src="https://user-images.githubusercontent.com/88386173/162730601-2a1c4f6a-edb5-4150-8d68-1899c94d949a.JPG" />
</p>

Shot entspricht die Globulis, die willkürlich durch den Screen geschoßen werden und ein weiteres Hindernis des Spiels darstellen sollen. Der erste Teil des Codes, greift die vom Shooter gegebene Ausrichtung auf und übertragt diese auf unser zu schießendes Objekt. "delete" und "mover" sind der Übersicht halber im public void act() und werden nacheinander ausgeführt.
 
<p align="center">
<img width="750" alt="delete" src="https://user-images.githubusercontent.com/88386173/162730641-fc378b4b-c9d7-40e4-8fd8-5ef08f9318ae.JPG" />
</p>
 
Wenn Shot auf den Protagonisten unseres Spiels, den Antikörper, trifft, wird der folgende Code ausgeführt. Der Abstand zum Antikörper ist in einem solchen Fall Null. Wenn der Abstand Null ist, wird der Antikörper aus der Welt gelöscht und es erscheinen die traurige Musik und der Loose-Screen, da man das Spiel bei Kontakt mit den Globulis verliert. 

<p align="center">
<img width="750" alt="mover" src="https://user-images.githubusercontent.com/88386173/162730693-9272250f-c732-4c3b-b3cf-a0dc409be736.JPG" />
</p>
 
Der Code für ,mover' sorgt dafür, dass sich unser Actor überhaupt bewegt und schlußendlich beim Aufprallen gegen die Ränder des Screens, nicht an diesen hängen bleibt und aus der Welt verschwindet. 

## NewGame
 
<p align="center">
<img width="100" alt="PlayAgain" src="https://user-images.githubusercontent.com/88386173/162730888-746e34e3-d882-4ffb-90f6-2a97e0a4296b.png" />
</p>
 
<p align="center">
<img width="750" alt="AllgPlayAgain" src="https://user-images.githubusercontent.com/88386173/162730830-23d5e9da-3bfb-4855-9cc8-1ed96677b7de.JPG" />
</p>
 
Im Code des Actors ‚PlayAgain‘ wird am Anfang erst das Bild genau definiert. Dann kommt die Act Methode, in welcher definiert ist, dass wenn man mit der Maus den Actor klickt, ein Klick-Geräusch abgespielt und der GameScreen geöffnet wird. Man kann das Spiel direkt erneut starten und so die Animation und Anleitung am Anfang überspringen.


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
Antonia hat zu Hause, da sie krank war und in ein paar Stunden gefehlt hat, weiter gearbeitet. Zum einen hat sie Github aktualisiert und den Aufbau der Seite weiter ausgearbeitet. Dann hat sie im Greenfoot Buch erste Codes herausgesucht, die für unser Spiel nützlich sein könnten. Zuletzt hat sie unseren Spielhintergrund und die Charaktere gezeichnet, sodass wir diese ins Spiel einarbeiten können.
Farhat hat zu Hause, da sie krank war, für Antonia und Vanessa mögliche Codes recherchiert für die Art von Spiel, die wir umsetzen wollen.
In der Stunde haben wir angefangen, eine zweite Version von unserem Spiel zu programmieren. Der Unterschied zur anderen Version liegt dabei, dass sich der Protagonist nicht vor und zurückbewegt, sondern er sich ständig fortbewegt und man mit den links und rechts Tasten  nur der Winkel ändern kann. Zusätzlich zu der Steuerung haben wir auch schon den Antagonisten erstellt, welcher, wenn der Protagonist ihn berührt, verschwindet. Der Antagonist bewegt sich von alleine und völlig zufällig vortwärts und dreht um, wenn er den Bildschirmrand berührt. 
Bisher sind unsere Actors nur durch "Platzsteller" besetzt, da die Bilder, die Antonia zu Hause erstellt hat momentan noch nicht funktionieren. Sie haben, obwohl sie freigestellt sind, immer noch einen weißen Rand und erscheinend viel zu groß. Dieses Problem wollen wir noch lösen. 
  
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
  
Und hier sieht man nun final unseren ersten Entwurf des Spieles. Das Mader-ähnliche Tier stellt den Gegner dar, das K steuert der Spieler. Wichtig zu erwähnen ist hier, dass alles, sowohl die Kostüme der Actors als auch der Hintergrund bisher nur Platzhalter sind und sich noch ändern sollen.
  
Zusatz: Da Vanessa und Antonia  sich falsch verstanden haben und an zwei verschiedenen "Arten" des Spiels gearbeitet haben (vgl. 08.02.2022), mussten wir sämtliche Codes, die Vanessa eigentlich programmiert hatte, verwerfen.
  
Vanessa hat also Plan geändert und die Rollen von "pizza" und "leaf" umgedreht. "Pizza" soll jetzt das Antikörper sein, welches vom Actor "leaf", unserem Aluhütchen, abgeschossen werden soll. Die Funktionen, des sich Hoch- und Runterbewegens waren also nicht mehr nötig, genauso wie das weitere Programmieren des sich automatisch Hoch- und Runterbewegenden "leaf"-Actor. Nachdem Antonia und Vanessa das Missverständnis geklärt haben und sich dazu entschieden haben, an Antonias "Jagd"-Version weiter zu codieren, hat sich Vanessa mit unterschiedlichen Codes auseinandergesetzt, die man in die richtige Version einsetzen könnte. Der nächste Schritt war für sie, ein Code zu finden, durch welchen der Actor "pizza" verschwindet, sobald er vom abgeschossenen Actor "Shots" berührt wird. 
  
Code für das Verschwinden von "pizza" nach dem Abschießen von "Shots":
  
![shotnewcode](https://user-images.githubusercontent.com/88386321/157477273-3c111640-72f4-4b73-8a77-35ed253a602f.jpeg)


## 09-02-2022
Vanessa und Antonia haben sich aufgeteilt und coden jeweils beide an einer der beiden App-Versionen weiter. Am Ende wollen wir dann die Funktionen, die uns am besten gefallen, zu einem Spiel zusammensetzen. 
So hat Vanessa weiter an einer "Schieß-Funktion" gecodet, die wir später für Hindernisse nutzen wollen, die auf unseren Protagonisten schießen, oder er kann auf diese schießen.
Antonia hat währenddessen eine zweite subworld erstellt und auf dieser einen Startbutton-actor eingeführt, bei welchem auf Knopfdruck das Spiel startet. Da Greenfoot andauernd abgestürzt ist, konnte sie ihn bisher nicht testen und muss dies nächste Stunde tun. Zuhause hat Antonia den GitHub für die letzten Tage geupdatet.

## 15-02-2022
Antonia hat einen Start Screen als neue World eingefügt, die als Erstes erscheint, wenn man das Spiel startet. Darauf ist ein Actor mittig platziert, welcher wie ein Startknopf aussieht. Wenn man auf "Button" drückt, erscheint der Gaming Screen und der Coronavirus fängt schon an sich zu bewegen. 
Den Actor, den der Spieler selbst steuert, ein Antikörper, fängt erst an sich zu bewegen, wenn man die Eingabetaste klickt. Dies haben wir mit einer Boolean Funktion codiert, die immer false ist, außer wenn die Eingabetaste gedrückt wird. Und die Aktionen des Antikörper arbeiten nur, wenn Boolean true ist. 
Nachdem dies eingestellt war, hat sich Antonia an die Einführung eines Hindernis probiert. Wir wollten Querdenker, sogenannte "Alu"s (wegen Aluhüte), die immer wieder random auftauchen und nach ein paar Sekunden wieder verschwinden. Wenn der Antikörper gegen einen Alu stößt, ist das Spiel verloren.
Der Code sieht vor, dass  der Computer eine Zahl zwischen 0 und x random generieren soll. Ist diese Zahl 15, wird ein Alu an eine beliebige Stelle im Spiel platziert. Allerdings hat sie dazu noch nicht die Funktion erstellt, dass Alu nach ein paar Sekunden wieder verschwindet, weshalb sie in der Test- und Suchphase nach einer passenden Zahl, von Alus überschwemmt wurde. Doch nach ein paar Versuchen, hat sie eine gute Zahl gefunden, wo Alus in einem angemessenen Abstand spawnen.
  
<p align="center">
<img width="700" alt="startbutton" src="https://user-images.githubusercontent.com/88386173/156214139-04980902-3b87-42fd-bec8-1a2497f6e4b9.PNG" />
</p>
Dies ist der StartButton, der das Spiel startet.
  
  <p align="center">
<img width="700" alt="gegner" src="https://user-images.githubusercontent.com/88386173/156213672-2d6295b6-b3cb-4e48-82a2-829dd9057b8e.PNG" />
</p>
  
Dies ist der Code, damit Gegner nach einer zufälligen Zeit auftauchen und das Spiel verloren ist, wenn der Antikörper ein Alu berührt.

Vanessa hat sich mit der Frage beschäftigt, wie die Shots, nachdem sie geschossen wurden, verschwinden können. Nach dem Abschießen blieben diese am Rand des Spiels hängen, was ja im wahren Spielen vermieden werden sollte. Sie hat sich also im Forum und in der Greenfoot-Bibliothek über mögliche Codes informiert und auch verschiedene ausprobiert. Jedoch hat keiner von diesen funktioniert. Ihre Aufgabe war es also, nach einem passenden Code zu suchen. Weiter beschäftigt sich Vanessa auch mit der Frage, wie "Shots" automatisch geschossen werden kann, da diese Funktion zu einem Actor gehört, den wir nicht kontrollieren sollen, sondern der den Spieler in verschiedenen Zeitabständen abschießen soll.
  
## 16-02-2022
Antonia hat heute den Start-Button auf dem Startscreen resized, da dieser viel zu groß war. Dazu hat sie die beiden End-Screens 'Loose' und 'Win' provisorisch erstellt und in das Spiel eingebettet. Bis zur nächsten Stunde will sie die endgültigen Screens für das Ende designen.   
Farhat war heute auch wieder da und schaut uns über die Schulter. Zusätzlich probiert sie sich selbst im Programmieren und recherchiert im Internet nach nützlichen Codes.
  
<p align="center">
<img width="500" alt="startbuttonsize" src="https://user-images.githubusercontent.com/88386173/156215523-88df1fe1-7f48-4fac-b59a-f9c46c3ac9d1.PNG" />
</p> 
Dieser Code passt die Größe des Buttons an.
  
Vanessa hat zusammen mit Herrn Buhl den richtigen Code zum Verschwinden von "Shots" am Rand gefunden und diesem im Spiel eingebaut (einen Code, den sie unter anderem schon probiert hatte, jedoch falsch programmiert hatte). Außerdem hat sie eine Lösung gefunden, wodurch "Shots" in bestimmten Zeitabständen vom Actor "leaf" geschossen werden kann. Diesen Code plant sie nächste Stunde zu programmieren.
  
![shotnewcode](https://user-images.githubusercontent.com/88386321/157490166-a99244e7-9ea2-4947-a0ad-9d43e904a691.jpeg)

Code der "Shots"-Klasse zum Verschwinden 
  
## 22-02-2022
Antonia hat bei den Alus (die Hindernisse) nun versucht einen Timer einzuführen. Wenn dieser abgelaufen ist, soll das spezifische Alu wieder verschwinden. Allerdings scheint irgendwo im Code ein Fehler zu liegen, den sie partout nicht finden kann. Denn anstatt nach einigen Sekunden zu verschwinden, verschwindet Alu sofort und taucht auch nie wieder auf. Da sie den Fehler im Code vorerst nicht finden kann, macht sie erstmal was anderes. Sie führt die endgültigen Loose- and Win-Screens ein. Auch ändert sie vom Antikörper das provisorische Kostüm (ein roter Kreis mit "K" drin) zu dem endgültigen Kostüm, dass sie extra zu Hause gezeichnet hat.

Vanessa hat hingegen die Funktion zum automatischen Schießen von "Shots" codiert. Dafür hat sie in der Bowser-Klasse von "leaf" die Maximale und Minimale Verzögerung zwischen den Schüssen angegeben, wobei sie die Parameter 40 und 160 gewählt hat. Der Timer, welche die Funktion "shoot()" der "leaf" Klasse aufruft, besteht aus der Summe von dem Minimalwert (40) und eine willkürliche Zahl zwischen den Parametern, wobei diese Funktion wiederholt läuft.
  
![leafcodenew](https://user-images.githubusercontent.com/88386321/157482899-57747368-0619-40a3-b1b0-5dbda127a2e0.PNG)

Erste Code: Timer der "Shots"
  
## 23-02-2022
Herr Buhl hat Vanessa und Antonia eine weitere, ausführlichere Ausführung in Greenfoot gegeben und ihnen weitere Codes und Möglichkeiten präsentiert. Auch hat er den Fehler in Antonias Alu-Timer gefunden (ein ";", wo es nicht hingehörte). Der Code funktioniert nun also.
  
<p align="center">
<img width="700" alt="timer" src="https://user-images.githubusercontent.com/88386173/156214506-92c66ef4-94ee-4874-b7e4-75f6f6990f08.PNG" />
</p>
  
Das fehlerhafte Semikolon kann man in der if Funktion sehen. Ohne dieses funktioniert der Code.
  
Herr Buhl konnte Vanessa mit dem Problem der willkürlichen Schüsse helfen. Da "Shots" nicht nur horizontal und in eine Richtung geschossen werden sollte, sondern in mehreren Richtungen, bedarft es auch einen entsprechenden Code. Vanessa hatte zunächst vor, mit der Funktion Greenfoot.getRandomNumber einen Code zu erstellen, durch welchen eine willkürliche Nummer ausgesucht werden solle, die durch andere Codes eine Schussrichtung angeben sollte. Dies hatte leider nicht funktioniert. Dennoch konnte Herrn Buhl uns dabei helfen, einen anderen Code zu finden.
  
![shotnewcode](https://user-images.githubusercontent.com/88386321/157486181-e1497787-44db-4ec1-b6de-a205c3cb10f4.PNG)

Der Code gehört zur "Shots"-Klasse. Der obere Teil in der Bowser-Klasse gehört zur Ausführung der Funktion. Der Code der "leaf"-Klasse ruft die Funktion für den Actor "Shots" auf.
  
![leafcodenew](https://user-images.githubusercontent.com/88386321/157486779-1d5f9549-15e1-44bd-8907-e5eade30cbbb.PNG)

Der zweite Code gehört zu "leaf" und basiert auf dem schon erahnten Prinzip von "Greenfoot.getRandomNumber". Er dient zur willkürlichen Schieß-Funktion von "leaf"

  
## 01-03-2022
Antonia hat zu Hause den GitHub aktualisiert und die Sachen eingetragen, die sie in den letzten 2 Wochen programmiert hat. Sie hat auch einen neuen Start-Screen designt. Im Unterricht hat sie dann direkt den neuen Start-Screen eingeführt. Dann hat sie eine kleine Animation programmiert, die abläuft, nachdem man den StartButton gedrückt hat (dieser verschwindet dann). Eine Spritze erscheint im Bild und bewegt sich nach links. An einer bestimmten Koordinate (X/Y), setzt sie ein Antikörper in die Welt (der Körper ist nun geimpft). Die Spritze bewegt sich weiter, bis sie den linken Rand berührt, dann öffnet sich das eigentliche Spiel. Nachdem dies funktioniert hat, hat sie das provisorische Corona Kostüm gegen das Echte ausgetauscht. Danach wurden alle Actors so unbenannt, dass sie am Anfang großgeschrieben werden und dementsprechend die Codes noch überarbeitet.
Farhat hat als Erstes nach einem Bild für unseren Alu-Actor gesucht. Danach hat sie auch gecodet. Sie hat ausprobiert, wie man Soundeffekte bei bestimmten Interaktionen und allgemein eine Melodie im Hintergrund einrichten kann. Dies wollen wir, wenn die Zeit es zulässt, noch auf unser Spiel übertragen.
Zum Schluss der Stunde hat Vanessa das erste Mal probiert, die separat programmierten Codes zusammenzufügen. Dies heißt konkret, dass wir Alu jetzt auch schießen lassen wollen. Die Codes an sich haben keine Fehler, aber sie funktionieren zusammen nicht so gut, wie einzeln. Wir werden nun versuchen, den Fehler zu finden. Sonst haben wir die Idee, dass wir 1 statischen Alu zusätzlich einführen, der immer da ist, und als einziger schießt. An diese Funktion soll nun Vanessa arbeiten.

<p align="center">
<img width="500" alt="neuerbutton" src="https://user-images.githubusercontent.com/88386173/156214849-93ae399c-836e-4dd4-a684-2fcf001d4ec2.PNG" />
</p> 
  
Der StartButton wurde für die Animation am Anfang umfunktioniert. Wenn dieser geklickt wird erscheint nun nicht direkt die Game-World, sondern der Knopf verschwindet und eine Spritze erscheint. 
 
<p align="center">
<img width="700" alt="Spritzecode" src="https://user-images.githubusercontent.com/88386173/156215546-19f20811-6cd7-43c5-9f5f-dd658dcce9c3.PNG" />
</p> 
  
Dies ist der Code für den neuen Actor "Spritze". Die Spritze bewegt sich nach links (also auf der X-Achse immer minus 1) und auf dem Weg setzt sie bei 200/200 ein Antikörper ab, der Körper ist nun also "geimpft". Wenn sie den Rand berührt (ifAtEdge), wird das eigentliche Spiel gestartet.

## 02-03-2022
Da wir mit der Entwicklung des Spiels schon ziemlich weit sind und planen, in der nächsten Doppelstunde den Fehler der Alus zu beheben, haben sich Antonia und Vanessa zusammengesetzt, um weitere Ideen für das Spiel zu konzipieren. Sie sind zu dem Entschluss gekommen, dass sie den von Farhat gesuchten Code für Soundeffekte einbauen wollen und auch an eine Funktion arbeiten wollen, die Schriftzüge (z.B. Hilfe, rette mich vor Corona!) einblenden lässt. Letztere Funktion wird sich Antonia widmen während Vanessa probiert den Fehler zu beheben. Außerdem hat Vanessa diese Stunde sämtliche Screenshots von Codes gemacht und einige alte Codes nachgestellt, die sie vergessen hatte, zu screenshoten.
 
## 08-03-2022
Heute ist der Unterricht wegen eines Ausfluges ausgefallen.
  
## 09-03-2022
Heute hat sich Vanessa weiterhin mit dem Problem der Aluhütte beschäftigt. Die verschiedenen Codes hat sie alle abgeglichen und verschiedene Fehler (falsche Benennung der Actors) korrigiert. Es scheint jedoch, dass es immer noch zu Fehler kommt, weswegen wir nun beschlossen haben, zwei verschiedene (Alu-)Actors zu erstellen, von denen einer die programmierte Schießfunktion besitzt und der andere willkürlich, als Hindernis, spawnt. Zudem hat Vanessa Zuhause ihre fehlende Einträge nachgetragen und den Github vervollständigt.   
Antonia hat versucht, einen Code zu programmieren, um einen bestimmten Text am Anfang des Spieles erscheinen zu lassen. Nebenbei hat sie Farhat dabei unterstützt, Codes auszuprobieren, die Soundeffekte oder Hintergrundmelodien erscheinen lassen.

## 15.03.2022
Antonia hat zu Anfang der Stunde die Lösung für den Text gefunden und ihn auch in das Spiel eingebaut.
Vanessa hat währenddessen das Zusammenführen beider Versionen des Spiels, die wir programmiert haben, wiederholt, da beim ersten Mal irgendwo ein Fehler geschehen ist. Am Ende haben wir alle am Spiel gearbeitet und die Funktionen aller Actors geprüft. Das Zusammenführen der Codes hat geklappt und die Roh-Version unseres Spieles funktioniert.
 
## 16.03.2022

 
## 22.03.2022
Wir wollen einen Text als Anleitung (zum Beispiel "Steuer mit den Pfeiltasten") am Anfang des GameScreens erscheinen lassen. Dieser soll aber auch wieder verschwinden (zum Beispiel, wenn man enter drückt, oder nach einer bestimmten Zeit). Wir haben sowohl eine if (-else) Funktion, als auch  Boolean ausprobiert, doch dies führte beides nicht zu dem gewünschten Ergebnis. Unser Fehler war, dass wir dachten, dass wenn bei Boolean/if das andere erfüllt wird, das Erste dann verschwindet. Doch so ist es nicht. Wir hätten zwar auch mit einem Image arbeiten können, haben uns aber dagegen entschieden und stattdessen den Text auf den StartScreen gepackt. Dort verschwindet er automatisch, sobald ein neuer Screen (Game Screen) geöffnet wird.
 
<p align="center">
<img width="600" alt="text" src="https://user-images.githubusercontent.com/88386173/162736254-b51afb5b-9ebd-4776-b821-97e41edf1f39.JPG" />
</p>

## 23.03.2022
Frei wegen der mündlichen Englisch Prüfungen
 
## 29.03.2022
Letzte Informatikstunde. Vanessa und Antonia haben beide Corona. Farhat ist krank.
 
## 06.04.2022
Herr Buhl ist netterweise in die Schule gekommen. Somit konnten Vanessa und Antonia das Spiel einmal so abspeichern, sodass wir auch von zu Hause weiterarbeiten können. Außerdem hat auch er nochmal über unsere Codes geschaut und uns geholfen. So hat er uns in der Annahme bestätigt, dass wir das vorherige Textproblem wahrscheinlich nur mit einem Image lösen hätten können. 

## Osterferien
Wir haben die Sounds in das Spiel integriert. So gibt es jetzt ab dem Game Screen eine durchgehende Melodie im Hintergrund. Zusätzlich gibt es Klick-Geräusche, wenn man einen Knopf drückt und einen Applaus oder eine traurige Melodie, je nachdem, ob man verliert oder gewinnt.
Auch haben wir einen PlayAgainButton etabliert. Dieser erscheint auf dem Win- oder LooseScreen und ermöglicht ein schnelles Neustarten des Spieles. Da sich dabei aber die Hintergrundmusik selbst übereinandergelegt hat, mussten wir diese statisch codieren (Siehe Bild unten). Nun bleibt die Musik ab Spielbeginn durchgehend erhalten und startet nicht jedes Mal neu und überlagert sich dadurch selbst.
 
<p align="center">
<img width="600" alt="Static" src="https://user-images.githubusercontent.com/88386173/162736069-67aeada5-9358-43c8-be22-8be42da43765.JPG" />
</p>
 
Weiterhin haben wir, nachdem das Spiel fertig gestellt war, Screenshots von allen Codes erstellt und in Github eingearbeitet. Danach haben wir die Codes erklärt und das Fazit geschrieben.

</details>
  

### <a name="3"></a>Fazit

Obwohl dies bereits unser 2. Informatikprojekt war, hat es uns noch mal eine komplett neue Seite des Programmierens gezeigt. Da wir im letzten Projekt mit einer "Blocksprache" gearbeitet haben, war dieses Programmieren als Hinführung zur Java-Programmiersprache sehr geeignet. Es war eine super interessante erste Coding Erfahrung, und besonders Greenfoot war für alle Leistungsniveaus der Gruppe und für unser Vorwissen (das praktisch nicht vorhanden war) sehr angebracht. Zudem gab es in dem Greenfoot-Forum viele hilfreiche Tipps, weshalb das Codieren  nicht so schwer wie gedacht war.
Wenn wir unser fertiges Spiel nun genauer unter die Augen nehmen, sind wir sehr zufrieden. Wir waren sogar in der Lage mehr Funktionen, als zuvor geplant, einzubauen, wie zum Beispiel den Countdown und die Musik.
Gewiss hatten auch wir mal Probleme und mussten Codes mehrmals umschreiben, bis sie funktionierten, weshalb sie teils umständig wirken könnten. Wenn man noch ein Halbjahr hätte, könnte man vielleicht auch versuchen, einige Funktionen anders oder einfacher umzusetzen, zum Beispiel dass Alus auch schießen können und man dafür keinen extra Shooter Actor braucht. Dennoch ist unsere Umsetzung von Hindernissen schon besser, als wir sie am Anfang geplant hatten. Denn würden die Alus den Antikörper jagen oder es würde gezielt und nicht random geschossen werden, wäre es fast unmöglich gewesen, das Spiel zu gewinnen. 
Ein weiterer Aspekt, der gewiss auch interessant gewesen wäre, hätte man mehr Zeit gehabt, sind Level. Das Spiel ist auf diese Art und Weise jetzt natürlich nicht das spannendste der Welt und mit mehreren Leveln könnte es vielseitiger sein. Doch das zu programmieren und andere, verschiedene Gegner neu zu erstellen lag leider nicht im Zeitrahmen. 
Allem in allem sind wir sehr zufrieden mit unserer Leistung, besonders wenn man bedenkt, dass wir von 0 gestartet sind und nichts konnten. Wir haben immer Lösungen gefunden, wenn etwas nicht funktioniert hat und wir haben in dem Zeitplan, den wir erstellt haben, sogar mehr geschafft als geplant. Am Ende ist ein witziges, an 'Arcade-Spiele' erinnerndes Spiel entstanden, dass von vorne bis hinten funktioniert und in dem keine Spielrunde exakt gleich sind.

### <a name="4"></a>Finale Links

Notizen:
<p align="center">
<img width="250" alt="Actors" src="" />
</p>



