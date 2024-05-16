## LB 1 Vorbereitung


- **Entstehung des Begriffs "Cloud"**:
  - Der Begriff "Cloud" stammt aus der Computerwissenschaft und bezieht sich auf das Symbol eines Cloud-Symbols in Netzwerkdiagrammen, das das Internet darstellt. Die Idee war, Ressourcen und Dienste über das Internet zugänglich zu machen.

- **Definition von "Cloud" laut NIST**:
  - Gemäß dem National Institute of Standards and Technology (NIST) ist Cloud-Computing ein Modell, das jederzeit und überall bequemen, bedarfsgerechten Netzwerkzugriff auf einen gemeinsam genutzten Pool von konfigurierbaren Rechenressourcen bietet.

- **5 Merkmale einer Cloud**:
  1. On-Demand Self-Service
  2. Breitbandzugriff auf das Netzwerk
  3. Ressourcen-Pooling
  4. Elastizität
  5. Messbarkeit

- **Cloud-Dienstleistungen**:
  - Infrastructure as a Service (IaaS), Platform as a Service (PaaS), Software as a Service (SaaS), Function as a Service (FaaS), Database as a Service (DBaaS), Backup as a Service (BaaS), Security as a Service (SECaaS), usw.

- **Cloud-Anbieter**:
  - Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform (GCP), IBM Cloud, Oracle Cloud, Alibaba Cloud, usw.

- **Cloud-Deployment-Modelle**:
  - Public Cloud, Private Cloud, Hybrid Cloud, Community Cloud

- **Cloud-Service-Modelle**:
  - Infrastructure as a Service (IaaS), Platform as a Service (PaaS), Software as a Service (SaaS), Function as a Service (FaaS)

- **Vorteile des Cloud-Computings**:
  - Skalierbarkeit, Flexibilität, Kostenersparnis, Zugänglichkeit, Automatisierung, Schnelligkeit der Bereitstellung von Ressourcen

- **Nachteile des Cloud-Computings**:
  - Datenschutz- und Sicherheitsbedenken, Abhängigkeit vom Internet, Compliance-Herausforderungen, mögliche Leistungsprobleme

- **On-Premise-Dienstleistungen**:
  - In Ihrem Betrieb werden wahrscheinlich Dienste wie interne Datenbanken, lokale Anwendungen und spezialisierte Systeme On-Premise betrieben.

- **Teilen technologischer Beiträge in der Cloud**:
  - Technologische Beiträge können über Plattformen wie GitHub durch das Erstellen und Veröffentlichen von Repositories geteilt werden. Klare Dokumentation, Readme-Dateien und Lizenzierung sind entscheidend für eine strukturierte und transparente Bereitstellung.

  ## Auftrag 3.1: Grundlagen Container-Technologie


- **Was ist Container-Technologie oder Container-Virtualisierung?**

    Container-Technologie ist eine Form der Virtualisierung, bei der Anwendungen und ihre Abhängigkeiten in isolierten Containern ausgeführt werden, die auf einem gemeinsamen Betriebssystemkern laufen.

- **Vor- und Nachteile der Container-Technologie im Vergleich zu virtuellen Servern (VM)**

    Vorteile:
        Schnellere Bereitstellung
        Geringerer Ressourcenverbrauch
        Höhere Effizienz
        Bessere Portabilität
    Nachteile:
        Geringere Isolation
        Begrenzte Unterstützung für bestimmte Betriebssysteme
        Komplexität bei der Verwaltung von Containern

- **Produkte im Zusammenhang mit virtuellen Servern und Containern**

    Virtuelle Server:
        VMware vSphere
        Microsoft Hyper-V
        KVM
        VirtualBox
    Container:
        Docker
        Kubernetes
        Docker Swarm
        OpenShift

- **Unterschiede zwischen VM und Container in Bezug auf Bereitstellung, Speicherplatz, Portabilität, Effizienz und Betriebssystem (Kernel)**

    Bereitstellung: VMs benötigen mehr Zeit, während Container nahezu sofort bereit sind.
    Speicherplatz: VMs benötigen mehr Speicherplatz, da sie ein eigenes Betriebssystem und Kernel enthalten, während Container Ressourcen teilen.
    Portabilität: Container sind portabler, da sie Anwendungen und ihre Abhängigkeiten kapseln, während VMs ganze Betriebssysteme umfassen.
    Effizienz: Container sind effizienter in Bezug auf Ressourcennutzung.
    Betriebssystem (Kernel): VMs verwenden eigene Betriebssysteme und Kernel, während Container den Kernel des Host-Betriebssystems nutzen.

- **Können virtuelle Server immer durch Container ersetzt werden?**

    Nicht immer. Container eignen sich gut für bestimmte Arten von Anwendungen, aber es gibt Fälle, in denen die Isolation und die Ressourcentrennung von VMs erforderlich sind.

- **Unterschied zwischen Self-Managed und Fully Managed**

    Self-Managed: Benutzer sind für die Bereitstellung, Konfiguration, Überwachung und Wartung der Infrastruktur verantwortlich.
    Fully Managed: Der Anbieter übernimmt die Verantwortung für die Bereitstellung, Konfiguration, Überwachung und Wartung der Infrastruktur, wodurch Benutzer entlastet werden.

    ## Auftrag 4.1: Container-Orchestrierung

- **Warum braucht man Container-Orchestrierung?**
        Um komplexe Anwendungen, die aus mehreren Containern bestehen, effizient zu verwalten, zu automatisieren, zu skalieren und zu überwachen.
        Um Hochverfügbarkeit, Lastenausgleich und Flexibilität zu gewährleisten.

- **Wie funktioniert Container-Orchestrierung?**
        Container-Orchestrierung verwaltet automatisch das Deployment, die Skalierung, das Load Balancing, die Wiederherstellung und die Aktualisierung von Containern über eine zentrale Plattform oder Software.

- **Welche Container-Orchestrierung Technologien kennen Sie?**
        Kubernetes
        Docker Swarm
        Apache Mesos
        Amazon ECS (Elastic Container Service)
        Google Kubernetes Engine (GKE)
        Azure Kubernetes Service (AKS)

- **Was versteht man unter "Scaling Containers"?**
        "Scaling Containers" bezieht sich auf die Fähigkeit, die Anzahl der laufenden Containerinstanzen basierend auf dem aktuellen Ressourcenbedarf automatisch zu erhöhen oder zu verringern.

- **Was gibt es für Deployment Strategien?**
        Blue-Green Deployment: Es werden zwei parallele Umgebungen betrieben, wobei eine aktiv ist (Blue) und die andere aktualisiert wird (Green), dann wird der Verkehr umgeleitet.
        Canary Deployment: Eine neue Version der Anwendung wird schrittweise auf einem kleinen Teil des Traffics getestet, bevor sie auf die gesamte Produktionssite übertragen wird.
        Rolling Deployment: Neue Versionen werden schrittweise auf Teilen der Infrastruktur bereitgestellt, wobei alte Instanzen durch neue ersetzt werden, um Ausfallzeiten zu minimieren.

