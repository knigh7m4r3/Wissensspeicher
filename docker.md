Docker - CheatSheet
====================

## Run und Build
###docker build  
Baut anhand einer Dockerfile ein Image.  
Beispiel:  
`docker build --no-cache -t DOCKERFILE . --build-arg ARG=VALUE`  

| Schalter	|	Parameter	|	Effekt / Nutzen |
| ---	|	---	|	---|
| -t	|	DOCKERFILE . 	|	Auswahl der Dockerfile - PUNKT NICHT VERGESSEN!	|
| --build-arg	|	ARG=VALUE	|	Fügt Argument ARG mit VALUE hinzu |
| --no-cache	|	---	|	Zwingt neues Laden der benötigten Daten	|


###docker run  
Baut aus einem Image einen Container und startet diesen durch seinen Entry-Point  
 Beispiel:  
`docker run -p IN:OUT -d --name NAME dockerfile`  

| Schalter	|	Parameter	|	Effekt / Nutzen |
| ---	|	---	|	---|
| -p	|	IN:OUT	|	Portfowarding|
| -d	|	---	|	Container wird im Hintergrund ausgeführt|
| --name | NAME | Container wird nach NAME benannt|


## Container - Befehle
| Befehl | Nutzen |
| --- | --- |
| `docker ps -a` | Container anzeigen |
| `docker rm XY` | Container XY entfernen |

## Image - Befehle
| Befehl | Nutzen |
| --- | --- |
| `docker image ls` | Images auflisten |
| `docker rmi XY` | Image XY entfernen |


