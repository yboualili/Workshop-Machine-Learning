# Fallstudie Entwicklungswerkzeuge WS 2019 - TensorFlow

## Projekt

Als Aufgabe hatten wir einen Workshop über Entwicklungswerkzeuge erstellen.
Wir haben uns als Thema Machine Learning with Tensorflow ausgewählt.
Bis zu diesem Zeitpunkt hatten wir noch keine Vorlesung über Data Science/Machine Learning.

Bachelor 4. Semester

## Konfiguration
### 1. Ordnerstruktur anlegen
1. Dieses Repository als ZIP-Archiv [herunterladen](https://gitlab.win.hs-heilbronn.de/vweber/fsew-ws19-tensorflow/-/archive/master/fsew-ws19-tensorflow-master.zip) und in den Ordner entpacken
2. [Cats vs Dogs Dataset](https://www.microsoft.com/en-us/download/confirmation.aspx?id=54765) herunterladen und entpacken
3. Die Archivordner *Cat* und *Dog* in den Ordner `Data` kopieren
	

### 2. Python Version überprüfen
1. Konsole öffnen (Windows `cmd` ; Mac `Terminal`)
2. Python in Konsole starten (Windows: `py` ; Mac `python3` bzw. `python`
3. Wenn nicht Python 3.7.x in der 64-Bit Version vorhanden ist die entsprechende Version herunterladen & installieren
	* [Windows](https://www.python.org/ftp/python/3.7.5/python-3.7.5-amd64.exe)
	* [Mac](https://www.python.org/ftp/python/3.7.5/python-3.7.5-macosx10.9.pkg)

### 3. Virtuelle umgebung erstellen, aktivieren und Bibliotheken installieren
1. Konsole öffnen und in diesen Ordner navigieren
    * Dateipfad im Explorer/Finder kopieren und `cd <kopierter Pfad>` in Konsole eingeben
2. Neue Virtuelle Umgebung erstellen
    * **Windows:** `py -m venv .\venv`
    * **Mac:** `python3 -m venv .\venv` (evtl. python statt python3)
3. Virtuelle Umgebung aktivieren
    * **Windows**: `venv\Scripts\activate.bat`
    * **Mac:** `venv\bin\activate`
4. Bibliotheken installieren 
    * pip & setuptools updaten: 
        * **Windows:**: `py -m pip install --upgrade pip setuptools`
        * **Mac:** `python -m pip install --upgrade pip setuptools`
    * Bibliotheken installieren: `pip install -r requirements.txt`

### 4. Jupyter Notebook starten
1. Im Konsolenfenster `jupyter notebook` eingeben
    * Es sollte sich ein Browserfenster öffnen

### 5. TensorBoard Server starten
1. Neues Konsolenfenster öffnen und Virtuelle Umgebung starten
    * siehe Schritte 3.1 und 3.3
    * **WICHTIG:** Beide Schritte einzeln ausführen
2. `tensorboard --logdir Logs` eingeben
    * In einem neuen Browsertab `localhost:6006` öffnen
    * Hier dürften noch keine Daten zu sehen sein, das kommt später
