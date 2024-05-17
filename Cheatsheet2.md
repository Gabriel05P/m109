## Cheatsheet für Prüfung Theorie-Fragen

**Welche Cloud-Service Modelle haben wir?**

- IaaS
- PaaS
- SaaS
- FaaS

**Punkt 1.25**

**Welche von den Cloud-Service Modellen hat Kunde am meisten Kontrolle über Infrastruktur? Wo am wenigsten?**

- **IaaS** IaaS bietet Kunden die größte Kontrolle über die Infrastruktur, da sie virtuelle Maschinen, Netzwerke, Speicher und andere Ressourcen direkt verwalten können. Kunden haben die Flexibilität, Betriebssysteme, Anwendungen, Datenbanken und andere Softwarekomponenten nach ihren eigenen Anforderungen zu installieren und zu konfigurieren. Sie sind für das Patchen, Sicherheitsupdates und die Wartung der Infrastruktur verantwortlich.

- **FaaS** FaaS bietet Kunden noch weniger Kontrolle über die Infrastruktur im Vergleich zu anderen Modellen. Kunden laden einfach ihren Code hoch und lassen den Cloud-Anbieter die Ausführung und Skalierung der Funktionen verwalten. Kunden haben kaum Einfluss auf die zugrunde liegende Infrastruktur, Betriebssysteme oder Ressourcenallokation.

**Was ist eine Grundvoraussetzung / Grundtechnologie von der Technologie Cloud Computing?**

Eine grundlegende Technologie, die Cloud Computing ermöglicht, ist die Virtualisierung. Virtualisierung ist Basis von Cloud-Computing. Virtualisierung ist die Abstraktion von physischen Ressourcen wie Rechenleistung, Speicher und Netzwerkressourcen, um virtuelle Instanzen, Container und Functions dieser Ressourcen zu erstellen, die unabhängig voneinander betrieben werden können. (Hyper V Beispiel)

**Über welche Arten kann ich kommunizieren? Ressourcen bestellen / abbauen?**

- **GUI / Web-Benutzeroberfläche (Web-Portal):** Die meisten Cloud-Anbieter stellen eine webbasierte Benutzeroberfläche oder ein Portal bereit, über das Sie Ressourcen bestellen, konfigurieren und verwalten können. Diese Benutzeroberflächen sind benutzerfreundlich gestaltet und bieten eine grafische Darstellung der verfügbaren Dienste und Optionen.

- **Befehlszeilenschnittstelle (CLI):** Cloud-Anbieter bieten auch Befehlszeilen-Tools und -Clients an, mit denen Sie über die Befehlszeile mit der Cloud-Plattform interagieren können. Diese CLI-Tools ermöglichen es Ihnen, Befehle auszuführen, um Ressourcen zu erstellen, zu konfigurieren und zu verwalten, und sind oft in verschiedenen Programmiersprachen verfügbar.

- **API (Application Programming Interfaces):** Cloud-Anbieter stellen APIs bereit, die es Entwicklern ermöglichen, ihre eigenen Anwendungen oder Skripte zu erstellen, um mit der Cloud-Plattform zu interagieren. Diese APIs bieten eine programmatische Schnittstelle zur Bestellung, Konfiguration und Verwaltung von Ressourcen und können in verschiedenen Programmiersprachen verwendet werden.

**Was ist Cloud-Computing?**

Cloud-Computing ist ein Modell zur Bereitstellung von IT-Ressourcen und Diensten über das Internet. Anstatt physische Hardware oder Software lokal zu erwerben und zu betreiben, können Unternehmen und Einzelpersonen Cloud-Ressourcen von Cloud-Service-Anbietern mieten oder abonnieren. Diese Ressourcen können verschiedene Formen annehmen, einschließlich Rechenleistung, Speicher, Netzwerkressourcen, Datenbanken, Entwicklungsplattformen, Anwendungen und mehr.

Wir beziehen IT-Dienstleistungen, also Bereitstellungen von IT-Dienstleistungen.

**Was sind Nachteile?**

- Im Thema Skalierung möchten wir bei Cloud-Modellen möglichst auf Vertikale Skalierung verzichten. In der Cloud setzen wir eher auf Horizontal (Elastic Scaling)

- Abhängigkeit vom Internet.

- Daten oder sensible Daten betrachten, also die Datenhaltung

**Punkt 1.27**

**Was sind die Cloud-Bereitstellungsmodelle?**

Hybrid, Public, Private und Community. 

**Punkt 1.24**

**Produkte von Container Engines oder Container Runtime?**

- **Docker-Engine:** Docker Engine ist eine der beliebtesten Container-Runtime-Engines. Sie ermöglicht das Erstellen, Ausführen und Verwalten von Containern mit Hilfe der Docker-Plattform.

- **CRI-IO:** CRI-O ist eine Open-Source-Implementierung des Kubernetes Container Runtime Interface (CRI). Es ist darauf ausgerichtet, Containertechnologien in Kubernetes-Clustern zu unterstützen und bietet eine minimale Laufzeitumgebung für Container

- **Podman:** Podman ist ein Container-Management-Werkzeug, das es ermöglicht, Container ohne die Notwendigkeit eines zentralen Dämons (wie Docker) auszuführen und zu verwalten. Es ist in der Lage, Container mit der gleichen API und den gleichen Befehlen wie Docker auszuführen, bietet jedoch zusätzliche Funktionen wie das Ausführen von Containern als nicht-Root-Benutzer und die Integration mit systemd.

- **Buildah:** Buildah ist ein Werkzeug zum Erstellen von Containern ohne die Notwendigkeit eines Dämons oder einer laufenden Container-Engine. Mit Buildah können Benutzer Docker-ähnliche Build-Befehle verwenden, um Container-Images zu erstellen, ohne Docker oder einen ähnlichen Dämon ausführen zu müssen. Buildah ermöglicht es, Container-Images einfach und sicher zu erstellen, ohne Docker-ähnliche Abhängigkeiten zu haben.

- **containerd:** containerd ist ein Open-Source-Container-Runtime-Manager, der von Docker entwickelt wurde. Es bietet eine leichte und effiziente Plattform für das Ausführen von Containern und ist Teil des CNCF-Projekts (Cloud Native Computing Foundation).

**Punkt 3.17**

**Was sind Orchestration Modelle?**

Kubernetes, K3s, Openshift, Docker-Compose

**Punkt 3.17**

**Wie überwachen die grossen Provider es rechnerisch von Aussen, also nicht von meiner Sicht aus? WICHTIG**

- **Overprovisioning:** Overprovisioning bezieht sich auf die Bereitstellung von mehr Ressourcen (wie Rechenleistung, Speicher und Netzwerkbandbreite) als tatsächlich benötigt wird, um den aktuellen Workload zu bewältigen. Dieser Ansatz ermöglicht es Cloud-Anbietern, Engpässe und Überlastungen zu vermeiden, indem sie einen Puffer an zusätzlichen Ressourcen bereitstellen, um unerwartete Lastspitzen oder Anforderungen zu bewältigen. Durch die Verwendung von Überbereitstellung können Cloud-Anbieter eine hohe Verfügbarkeit und Zuverlässigkeit ihrer Dienste sicherstellen, auch unter schwankenden Arbeitslasten.

- **Overcommitment:** Overcommitment bezieht sich auf die Zuteilung von mehr Ressourcen, als tatsächlich physisch vorhanden sind, basierend auf der Annahme, dass nicht alle Ressourcen gleichzeitig genutzt werden. Cloud-Anbieter verwenden Overcommitment, um die Effizienz ihrer Infrastruktur zu maximieren und die Auslastung ihrer Ressourcen zu optimieren. Dies kann beispielsweise bedeuten, dass mehr virtuelle Maschinen auf einem physischen Host bereitgestellt werden, als dessen tatsächliche Kapazität, unter der Annahme, dass nicht alle VMs gleichzeitig maximale Ressourcen benötigen.

- **Economy of Scale:** Die Wirtschaftlichkeit der Skalierung bezieht sich auf die Vorteile, die durch die Massenproduktion und den Einsatz großer Infrastrukturen erreicht werden. Durch den Betrieb von riesigen Rechenzentren und das Bereitstellen von Ressourcen auf globaler Ebene können Cloud-Anbieter Skaleneffekte erzielen, die es ihnen ermöglichen, Kosten zu senken und Ressourcen effizienter zu nutzen. Sie können beispielsweise Hardwarekomponenten in großem Maßstab einkaufen, automatisierte Prozesse implementieren und Betriebskosten auf viele Kunden verteilen, um wettbewerbsfähige Preise anzubieten.

Diese Konzepte werden von großen Cloud-Providern wie Amazon Web Services (AWS), Microsoft Azure und Google Cloud Platform (GCP) angewendet, um ihre Rechenzentren effizient zu betreiben, Skalierbarkeit zu ermöglichen und wettbewerbsfähige Preise anzubieten. Durch die Kombination von Overprovisioning, Overcommitment und Skaleneffekten können sie eine hohe Leistung und Zuverlässigkeit ihrer Dienste gewährleisten und gleichzeitig die Betriebskosten optimieren.

**Google-Cloud gibt 4 Optionen, welche sind beliebte Dienstleistungen von Google Cloud?**

- Sales Force
- Nutanix AHV
- Kubernetes GKE (Google Kubernetes Engine)
- Microsoft Azure VM

Unter den genannten Optionen ist Kubernetes GKE (Google Kubernetes Engine) die beliebteste Dienstleistung von Google Cloud. Es ist eine verwaltete Kubernetes-Dienstleistung, die es Unternehmen ermöglicht, Containeranwendungen einfach und effizient in der Google Cloud auszuführen, zu verwalten und zu skalieren. GKE bietet Funktionen wie automatische Skalierung, Lastausgleich, Rollback-Funktionen und Integrationen mit anderen Google Cloud-Diensten.

**Hauptmerkmal von Cloud-Computing?**

- On demand self service
- Breiter Netzzugriff
- Ressourcen pooling
- Elastizität
- Messbare Dienste

Von NIST oder **Punkt 1.23**

**Ich will ein Repo herunterladen oder gleichzeitig das erste Mal initialisiert herunterladen?**

- **Repository herunterladen (clone):**
```bash
git clone <repository-URL>
```

- **Änderungen vornehmen:** Füge oder ändere Dateien in deinem lokalen Repository.
```bash
git add .
```
Dies fügt alle Änderungen im Arbeitsverzeichnis zur Staging-Area hinzu. Falls du nur bestimmte Dateien hinzufügen möchtest, kannst du ihre Namen anstelle von . verwenden.

- **Änderungen committen (commit):**
```bash
git commit -m "Deine Commit-Nachricht hier"
```

- **Änderungen hochladen (push):**
```bash
git push
```
Dies lädt deine lokalen Commits in das Remote-Repository hoch. 

- **Änderungen aus dem Remote-Repository abrufen (pull):**
```bash
git pull origin master
```
Falls es Änderungen im Remote-Repository gibt, die du herunterladen möchtest:

**Oder Einstieg**

**Zu welchem Cloud-Servicemodell gehören virtuelle Server?**

Virtuelle Server gehören zum Cloud-Service-Modell "Infrastructure as a Service" (IaaS). In diesem Modell werden virtualisierte Computing-Ressourcen wie virtuelle Maschinen (VMs), Speicher und Netzwerk bereitgestellt, die es Benutzern ermöglichen, ihre eigenen Anwendungen, Betriebssysteme und Software zu hosten, ohne physische Hardware oder Rechenzentren verwalten zu müssen.

**Zu welchem Cloud-Servicemodell gehören Container?**

Container gehören zum Cloud-Service-Modell "Container as a Service" (CaaS) oder "Platform as a Service" (PaaS), abhängig von der spezifischen Bereitstellung und Verwaltung der Container durch den Cloud-Anbieter.

- **Container as a Service (CaaS):** Bei CaaS werden Containerruntime-Umgebungen wie Docker-Container als Dienst bereitgestellt. Benutzer können Container innerhalb der CaaS-Plattform erstellen, verwalten und ausführen, ohne sich um die zugrunde liegende Infrastruktur kümmern zu müssen. Der Cloud-Anbieter übernimmt die Verantwortung für das Bereitstellen und Skalieren der Container-Plattform, während Benutzer ihre Anwendungen in Containern betreiben können.

- **Platform as a Service (PaaS):** In einigen Fällen können Container auch als Teil von PaaS-Diensten angeboten werden. In einer PaaS-Umgebung bietet der Cloud-Anbieter eine Plattform für die Entwicklung, Bereitstellung und Ausführung von Anwendungen, die auf Container basieren. Dies kann die Verwendung von Tools wie Kubernetes oder Docker Swarm beinhalten, um Container zu orchestrieren und zu verwalten, während der Cloud-Anbieter die zugrunde liegende Infrastruktur und Plattformdienste bereitstellt.

- **Was sind Pods?**

Pods sind grundsätzlich Container unter OpenShift. Im Deployment-YAML geben wir unter dem Wert "replicas" an, wie viele Pods tatsächlich erstellt werden sollen.