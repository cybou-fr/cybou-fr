# Stanislav Saveliev — Architecte logiciel & systèmes

**Architecture · Modernisation et migration · MVP · Cloud / Desktop · Systèmes distribués**

> **Un logiciel à concevoir, moderniser ou remettre sous contrôle ?**
> Je transforme un besoin complexe ou un existant difficile à faire évoluer en architecture compréhensible, plan de réalisation vérifiable et logiciel fonctionnel.

[**Me contacter sur Malt**](https://www.malt.fr/profile/stanislavsaveliev) · [Projets actifs](#projets-en-développement-actif--architecture-en-pratique) · [Méthode de migration](docs/METHODE_MIGRATION_FR.md) · [Site de présentation (sources)](docs/index.html)

<div align="center">
  <a href="https://github.com/cybou-fr/fortiq"><img alt="FORTIQ — référence graphique approuvée du desktop Linux distant, maquette de conception" src="https://raw.githubusercontent.com/cybou-fr/fortiq/main/docs/design/reference/fortiq-shell-master.png" width="720" /></a>
  <p><sub>FORTIQ — référence de design approuvée (et non capture d’une version qualifiée). Architecture et code disponibles dans le dépôt.</sub></p>
</div>

## Les missions sur lesquelles je peux vous aider

| Votre situation | Mon intervention | Livrables concrets |
| --- | --- | --- |
| **Une application existante devient fragile ou coûteuse à faire évoluer** | Audit technique, risques, dette, priorités et stratégie de modernisation | Cartographie, diagnostic, architecture cible, roadmap et première tranche d'amélioration |
| **Vous devez changer de langage, framework ou plateforme** | Migration progressive et protection des comportements métier et des données | Plan de migration, contrats, code migré, tests de non-régression, stratégie de retour arrière |
| **Vous souhaitez lancer un nouveau produit** | Cadrage, architecture proportionnée au besoin et développement d'un MVP | Spécifications, décisions d'architecture, prototype/MVP démontrable, tests et documentation |
| **Vous construisez un logiciel natif ou un système distribué** | Conception et développement C++/Qt, Go ou Rust, API, stockage et sécurité | Composants, protocoles, interfaces, intégration et validation technique |

J'interviens **personnellement**, de l'analyse initiale à la livraison. Je combine architecture et implémentation : pas de recommandations détachées du code, ni de code sans critères de validation.

## Projets en développement actif — architecture en pratique

**Ces projets sont des réalisations personnelles de R&D, et non des missions clients.** La sélection met en avant les dépôts où le développement technique est actuellement le plus actif (activité vérifiée fin octobre 2026, parmi les projets publics), pas un classement permanent. Code disponible, choix d'architecture et limites de validation restent consultables.

### 1. [FORTIQ — Bureau Linux natif, sans agent serveur](https://github.com/cybou-fr/fortiq)
**C++20 · Qt Quick / QML · libssh2 · Windows / Android · Opérations distribuées**

Un bureau graphique local pour travailler sur un hôte Linux distant via SSH, SFTP, PTY et tunnels — sans déployer de service propriétaire ni de bureau graphique distant. L'architecture relie plusieurs applications (Files, MDok, Terminal, Logs, Mail, System, Network, Database) à des contrôleurs C++ et à un modèle commun de tâches.

**Décisions remarquables :** identité de session explicite, gestion des résultats incertains après rupture réseau, opérations à risque protégées, séparation entre composants UX communs et logique métier, critères de recette indépendants de l'implémentation.

[Étude architecturale dans le README](https://github.com/cybou-fr/fortiq#system-architecture) · [Architecture](https://github.com/cybou-fr/fortiq/blob/main/docs/ARCHITECTURE.md) · [Matrice de qualification UX](https://github.com/cybou-fr/fortiq/blob/main/docs/DESKTOP_EXPERIENCE_RELEASE_MATRIX.md)

*Statut : prototype open source en développement actif ; qualification produit et validation multi-plateforme non terminées.*

### 2. [CybouDB — Moteur de données et portabilité bas niveau](https://github.com/cybou-fr/CybouDB)
**Assembly · ABI · CMake · SQL / vecteurs / files de tâches · Portabilité ARM64**

Un travail sur les frontières entre moteur de données, assembleur et plateformes : audit des dépendances d'architecture, contrats ABI, construction multiplateforme et chemin de portage ARM64. Le défi est de préserver le comportement et les invariants du moteur tout en séparant le cœur portable de ses optimisations spécifiques.

[Code et documentation](https://github.com/cybou-fr/CybouDB)

*Statut : développement actif ; le travail ARM64 ne doit pas être interprété comme une qualification Android de bout en bout.*

### 3. [CYBOU Browser — Permissions visibles et navigation maîtrisée](https://github.com/cybou-fr/CybouBrowser)
**C++20 · Qt WebEngine · QML · Threat modeling · Tests de sécurité**

Un navigateur natif dont l'interface rend visibles les capacités demandées par les sites. Architecture distinguant politiques, demandes observées, autorisations et utilisation effective ; contrôle des frontières de confiance et programme de vérification des risques.

[Étude de cas](https://github.com/cybou-fr/CybouBrowser/blob/main/docs/CASE_STUDY_FR.md) · [Preuves et limites](https://github.com/cybou-fr/CybouBrowser/blob/main/docs/ENGINEERING_QUALITY.md)

*Statut : alpha, développement actif ; aucune certification de sécurité revendiquée.*

### 4. [MUTYVA — Applications natives déclaratives](https://github.com/cybou-fr/mutyva)
**C++20 · Qt 6.12 / QML · SQLite · Ingénierie assistée par IA**

Un système local de composition d'applications à partir de composants déclaratifs : contrats de données, évolution contrôlée des interfaces et préservation des données utilisateur, sans devoir exécuter arbitrairement du code généré.

[Étude de cas](https://github.com/cybou-fr/mutyva/blob/main/docs/CASE_STUDY_FR.md) · [Architecture et risques](https://github.com/cybou-fr/mutyva/blob/main/docs/23_ARCHITECTURE_ASSESSMENT.md)

*Statut : prototype en développement ; qualification native encore à terminer.*

### Autres preuves techniques — projets antérieurs ou moins actifs

- **[ZFSCloud](https://github.com/cybou-fr/zfscloud)** — Go, gRPC/Protobuf, TLS/mTLS et orchestration de stockage ZFS. [Étude de cas](https://github.com/cybou-fr/zfscloud/blob/main/docs/CASE_STUDY_FR.md).
- **[ConfidIS OS](https://github.com/cybou-fr/ConfidIS)** — Rust, fragmentation chiffrée, erasure coding et distribution de données sensibles. [Étude de cas](https://github.com/cybou-fr/ConfidIS/blob/main/docs/CASE_STUDY_FR.md).
- **[Sodix](https://github.com/cybou-fr/sodix)** — utilitaires système et cryptographie en Rust.

Ces dépôts restent accessibles comme **références de compétences**, sans prétendre qu'ils sont prioritaires aujourd'hui. [Explorer tous les dépôts](https://github.com/cybou-fr?tab=repositories).

## Ma méthode d'ingénierie

**Comprendre → Évaluer → Arbitrer → Documenter → Implémenter → Tester → Transmettre.**

1. **Cadrer :** objectifs métier, contraintes, architecture existante et risques.
2. **Comparer :** alternatives, coûts, compromis et architecture cible proportionnée.
3. **Décider :** ADR, diagrammes, contrats, critères d'acceptation et stratégie de migration.
4. **Livrer :** tranche verticale fonctionnelle, revue de code, CI, tests et démonstration.
5. **Transmettre :** documentation exploitable, limites, dette résiduelle et étapes suivantes.

L'intelligence artificielle accélère l'analyse, la documentation, l'implémentation et les tests ; **les décisions, la validation du code et la responsabilité technique restent humaines**.

## Compétences principales

- **Langages et systèmes :** C++20, Go, Rust, Delphi, C#/.NET ; Linux et Windows.
- **Applications desktop :** Qt / QML, interfaces natives, composants et intégration système.
- **Cloud, réseau et données :** API/RPC, architectures distribuées, P2P, stockage, migration et fiabilité.
- **Qualité :** documentation d'architecture, ADR, tests de non-régression, CI/CD, threat modeling, sécurité pragmatique.

## Travaillons ensemble

**Audit et feuille de route · Architecture et documentation · Modernisation / migration · MVP et développement logiciel.**

Missions courtes ou longues, en collaboration directe, à distance. Contractualisation via Malt ; portage salarial possible selon le cadre de la mission.

**[Présenter votre projet sur Malt](https://www.malt.fr/profile/stanislavsaveliev)**

---

*Transparence : ce portfolio prouve des choix techniques observables dans des projets personnels. Il ne présente pas ces projets comme des livraisons clients, des produits certifiés ou des résultats de production non documentés.*
