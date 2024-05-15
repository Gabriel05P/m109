## Auftrag 4.2 Container Orchestration mit Docker Compose

Folgen Sie dem Tutorial https://docs.docker.com/compose/gettingstarted/
Erstellen Sie ein Diagram und beschreiben Sie die einzelnen verwendeten Container
Beantworten Sie folgende Fragen
        
    -Was ist Redis?
    -Welche Ports werden genutzt?
    -Was ist die Bedeutung von ENV im DOCKERFILE?


    Was ist Redis?
        Redis ist eine Open-Source-In-Memory-Datenbank, die als Datenstrukturserver fungiert. Sie unterstützt verschiedene Datentypen und bietet Hochverfügbarkeit, Skalierbarkeit und Persistenz.

    Welche Ports werden genutzt?
        Standardmäßig nutzt Redis den Port 6379 für die Kommunikation. Dieser Port kann jedoch konfiguriert werden.

    Was ist die Bedeutung von ENV im DOCKERFILE?
        Die ENV-Anweisung in einem Dockerfile wird verwendet, um Umgebungsvariablen zu definieren. Diese Variablen können dann während des Build-Prozesses oder beim Ausführen des Containers verwendet werden, um Konfigurationen anzupassen oder dynamische Informationen bereitzustellen.
