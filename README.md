>TESTE TEST TEST 
Universität der Bundeswehr München  
> ETTI 6 Software Engineering / Softwaretechnik  
> Prof. Dr. Andrea Baumann

Dieses Projekt dient als Vorlage für die Dokumentation im Secure Software Engineering Praktikum. 

# Inhaltsverzeichnis

[01_Besprechungsprotokolle](01_Besprechungsprotokolle/_Besprechungsprotokolle.md)

[02_Projekthandbuch](02_Projekthandbuch/_Projekthandbuch.md)

[03_Risikoliste](03_Risikoliste/_Risikoliste.md)

[04_Anforderungsspezifikation](04_Anforderungsspezifikation/_Anforderungsspezifikation.md)

[05_Architekturdokument](05_Architekturdokument/_Architekturdokument.md)

[06_Testspezifikation](06_Testspezifikation/_Testspezifikation.md)

Im Verzeichnis [resources](resources) findet sich weitere relevante Informationen, wie z.B. individuelle oder aktuelle Visual Paradigm Modelle (https://www.visual-paradigm.com). 

***Wichtige Hinweise für das Schreiben von Dokumenten mit Markdown***

Markdown (https://daringfireball.net/projects/markdown/ oder auf deutsch https://markdown.de) ist eine 
einfach Art formatierte Texte zu schreiben. Markdown geschrieben Texte werden z.B. in GitLab schon 
formatiert angezeigt oder können z.B. nach `latex` oder `pdf` konvertiert werden. 

Für die vorliegende Dokumentation bitte unbedingt folgende Regeln beachten, damit eine Konvertierung mit 
Hilfe der vorgegebenen sogenannten [GitLab-Pipeline](.gitlab-ci.yml) in `pdf` Dokumente (einigermaßen) funktioniert. 

- Für die Konvertierung in ein `pdf` werden alle `md`-Dateien in einem Verzeichnis in alphanumerischer Reihenfolge 
aneinandergehängt und dann nach `pdf` konvertiert. Dateien mit einem `_` am Anfang werden ignoriert. Für jedes
Verzeichnis wird ein `pdf` erzeugt. Es werden nur Verzeichnisse bearbeitet, die mit einer Ziffer `[0-9]` beginnen. 

- Zwischen die aneinandergehängten Dateien wird jeweils ein Seitenumbruch und die Möglichkeit zur 
Referenzierung ergänzt.

- Es kann auf einen anderen Abschnitt innerhalb eines Dokuments verwiesen werden, indem man auf eine 
Datei im selben Verzeichnis verweist (siehe Beispiel im Kapitel [Anwendungsfälle] 
(04_Anforderungsspezifikation/06_00_Anwendungsfaelle)). Diese Verweise sind später im `pdf` navigierbar.

- Als oberste Kapitelebene zwei Raute Zeichen `##` verwenden. Die erste Ebene `#` wird für das 
Inhaltsverzeichnis ignoriert. 

- ... *falls irgendetwas trotz Einhaltung diese Punkte nicht wie erwartet funktioniert, dann bitte 
unbedingt über `Mattermost` oder per Mail melden und nicht die Zeit mit Formatierung verschwenden!*

***Wichtige Hinweise für den Ablauf der GitLab-Pipeline***

Nach einem `push` auf das Repository wird der Job `site_build` der GitLab-Pipeline automatisch ausgeführt. 
Dieser Job wandelt mit Hilfe der Anwendung `pandoc` die `md`-Dateien in `pdf`-Dateien um und kopiert 
diese und im Verzeichnis vorhandene Dateien vom Typ `xlsx`, `ods`, `doc` und `pdf` in einen 
Ordner.

Die Ergebnisse der Umwandlung finden Sie, nachdem der Job beendet wurde, in GitLab. 
Zum Beispiel unter `Build` -> `Pipelines`, neben der obersten bzw. neuesten `passed` Pipeline ganz rechts auf 
das Download-Symbol klicken und `site_build:archive` auswählen. Oder auf `passed`, dann auf `site_build` und 
dann auf den `Browse` klicken um sich die Artefakte im Browser anzuschauen.

Der beiden Jobs `site_upload`und `site_release` der Pipeline werden durch das Anlegen eines neuen 
`Tag` zusätzlich zum Job `site_build` angestoßen. Der Job `site_upload` zipped die erzeugten Artefakte 
und legt das zip-File in der `generic`-Package Registry ab. Der Job `site_build` erzeugt ein Release.

Wenn Sie alle Dokumente für eine wöchentliche Abgabe fertig haben, dann erzeugen also einfach ein `Tag`.

*Tritt in der Pipeline ein Fehler auf, dann erhalten Sie von GitLab eine Mail. Falls Sie den Fehler 
nicht selbst beheben können, dann geben Sie bitte über `Mattermost` oder per Mail Bescheid. Bitte
nicht zulange damit beschäftigen und so Zeit verschwenden!*

***Die GitLab-Pipeline kann auch lokal ausgeführt werden (falls Sie sich dafür interessieren)***

**Voraussetzung:** Docker muss installiert sein (siehe https://docs.docker.com), die folgenden Kommandos müssen im 
VPN ausgeführt werden

**Wichtig zu wissen:** Es wird die Version generiert, die bei Ihnen lokal liegt und `commit`ed wurde.

1. Get image from docker and start gitlab-runner daemon in the repository's directory

```
docker run -d --name gitlab-runner --restart always -v $PWD:$PWD -v /var/run/docker.sock:/var/run/docker.sock gitlab/gitlab-runner:latest
```

2. Make working directory for gitlab-runner

```
mkdir -p gitlab-runner-dir
mkdir -p gitlab-runner-dir/runner--project-0-concurrent-0
```

3. Start executing job

```
docker exec -it -w $PWD gitlab-runner gitlab-runner exec docker site_build --cache-dir="$PWD"/gitlab-runner-dir --docker-cache-dir="$PWD"/gitlab-runner-dir --docker-volumes="$PWD"/gitlab-runner-dir --builds-dir="$PWD"/gitlab-runner-dir
```

4. Copy results to target directory

```
mkdir -p  target
cp gitlab-runner-dir/*/*/*/*/_generated/* target/.
rm -rf gitlab-runner-dir
```

5. Stop gitlab-runner daemon and remove container

```
docker stop gitlab-runner && docker rm gitlab-runner
```

