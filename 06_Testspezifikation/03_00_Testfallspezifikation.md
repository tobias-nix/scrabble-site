
## Testfallspezifikation

###	Komponententest

Im Rahmen des Praktikums werden die Komponententests mit Hilfe von JUnit-Tests durchgeführt. Dazu werden die 
Komponenten über die Schnittstellen, die die Komponenten anbieten bzw. nutzen, mit Hilfe von JUnit-Tests getestet. 
Die Junit-Tests finden sich direkt im Programmcode und werden durch die Entwickler verantwortet.

###	Integrationstest

Für die Integrationstests wird auf die jeweiligen Komponententests zurückgegriffen. Dazu werden meherer Komponenten
im Rahmen von JUnit-Tests kombiniert. Auch diese Tests finden sich direkt im Programmcode.

### Systemtests

Im Systemtest wird das gesamte System getestet und es kommt vorrangig auf die korrekte Funktionsweise bei korrekter 
Eingabe an. Zweitrangig wird überprüft, ob fehlerhafte Eingaben nicht zu einem Systemausfall und sinnvollen 
Benutzerrückmeldungen führen.

