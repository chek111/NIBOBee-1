ATMEL ATMega 16A - Die Steuereinheit des NIBOBee
================================================

.. _NIBOBee: http://www.nicai-systems.com/de/nibobee
.. _Arduino Umgebung: https://www.arduino.cc/en/Main/OldSoftwareReleases
.. _Link: https://www.roboter.cc/index.php?view=article&id=28&option=com_content&Itemid=1
.. _Video: https://www.youtube.com/watch?v=V8gdC8kDm24&feature=youtu.be

Was ist der ATMega 16A?
-----------------------

Der ATMega 16A ist ein Mikrocontroller, welcher sich frei
programmieren lässt in C, C++, ARDUINO, Java und ASSEMBLER.
Für unseren NIBOBee_ dient er als Steuereinheit der Motoren und
Signalverarbeitung verschiedener Sensoren.

Um einen ATMega programmieren zu können, bedarf es einiger Vorbereitungen:

1. Zuerst benötigt man die `Arduino Umgebung`_. Damit NIBORobolib richtig funktioniert,
   wird von Nicai-Systems empfohlen, ARDUINO Version 1.6.7 zu
   installieren. (Es funktioniert auch die aktuelle Version 1.8 unter MacOS.)

   Die Arduino 1.6.7 installieren, und sich merken, in welchen Ordner man es installiert hat.

2. Jetzt installiert man unter folgendem Link_ die nötigen Libraries und Treiber, um den NIBOBee zum Laufen zu kriegen.
   Nicht vergessen, den Installer für 64 Bit Windows (7, 8, 10) zu installieren.

   Diese Datei wird in den selben Ordner wie die Arduino-IDE installiert.
   Entstehen hierbei Probleme, so muss man die NIBOBee Bibliotheken manuell in den Arduino-Ordner kopieren
   (Dieser PC / Windows (C) (kann variieren) / Programme (x86) / Arduino / libraries)
	
   Gibt es jetzt immer noch Probleme, so führt man die NiboRoboLib 3.4.1 (64 bit) Setup.exe aus
   und stellt unter dem Punkt Modify sicher,
   dass bei dem Unterpunkt NiboRoboLib / ARDUINO 1.6.6 integration kein rotes Häckchen mehr vorhanden ist.

4. Jetzt sollte man Arduino starten können, und unter dem Punkt: Werkzeuge / Board / das
   Board "nicai-systems NIBObee robot" auswählen können.
   Nicht vergessen auch noch den Programmer auf "NIBObee & burger programmer (usbasp) umzustellen.
	

5. Ist der NIBObee fertig zusammengelötet und funktioniert auch beim Einschalten, 
   (Lampen gehen an, Sensoren reagieren auf Bewegung, Tastsensoren funktionieren...)
   so kann man ihn an den Computer anschließen. (nicht wundern, dass kein Port erkannt wird, es funktioniert auch so)
   
   Unter dem Punkt: Datei / Beispiele / NIBObee / Kalibrierung muss man den NIBObee nun kalibrieren.
   Kalibrierung anklicken, es öffnet sich ein neues Arduino Fenster, auf das kleine Häkchen (überprüfen) klicken, 
   danach auf Hochladen gehen und warten, bis sich der NIBObee neu kalibriert.
   Die Annäherungssensoren sollten nach der Kalibrierung deutlich besser funktionieren, als vorher.
   
   Jetzt kann man noch diverse Funktionen des NIBObees anhand der vorgegebenen Beispielen austesten.
   (Beispiel Ping Pong, Motorsteuerung etc.)


Erste Fahrversuche des NIBOBee
------------------------------

Jetzt kann man mit der Arduino Umgebung herumspielen, um den NIBOBee in der Gegend herum fahren zu lassen.
Falls der NIBOBee nicht geradeaus fährt, muss man entweder den linken oder rechten Motor schneller drehen lassen.
In diesem Video_ fährt der linke Motor mit dem Speed 400, der rechte mit 500.

.. raw:: html
        
        <iframe width="480" height="320" src="https://www.youtube.com/watch?v=V8gdC8kDm24&feature=youtu.be" frameborder="0" allowfullscreen></iframe>
        
        <p><em>Er hat ein Händchen</em></p>
