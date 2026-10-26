# Stanislav Saveliev — Architecte logiciel & systèmes

**Architecture · Modernisation et migration · MVP · Cloud / Desktop · Systèmes distribués**

> **Un logiciel à concevoir, moderniser ou remettre sous contrôle ?**
> Je transforme un besoin complexe ou un existant difficile à faire évoluer en architecture compréhensible, plan de réalisation vérifiable et logiciel fonctionnel.

[**Me contacter sur Malt**](https://www.malt.fr/profile/stanislavsaveliev) · [Voir les études de cas](#études-de-cas--preuves-techniques) · [Ma méthode](#ma-méthode-dingénierie)

## Les missions sur lesquelles je peux vous aider

| Votre situation | Mon intervention | Livrables concrets |
| --- | --- | --- |
| **Une application existante devient fragile ou coûteuse à faire évoluer** | Audit technique, risques, dette, priorités et stratégie de modernisation | Cartographie, diagnostic, architecture cible, roadmap et première tranche d'amélioration |
| **Vous devez changer de langage, framework ou plateforme** | Migration progressive et protection des comportements métier et des données | Plan de migration, contrats, code migré, tests de non-régression, stratégie de retour arrière |
| **Vous souhaitez lancer un nouveau produit** | Cadrage, architecture proportionnée au besoin et développement d'un MVP | Spécifications, décisions d'architecture, prototype/MVP démontrable, tests et documentation |
| **Vous construisez un logiciel natif ou un système distribué** | Conception et développement C++/Qt, Go ou Rust, API, stockage et sécurité | Composants, protocoles, interfaces, intégration et validation technique |

J'interviens **personnellement**, de l'analyse initiale à la livraison. Je combine architecture et implémentation : pas de recommandations détachées du code, ni de code sans critères de validation.

## Études de cas & preuves techniques

**Ces projets sont des réalisations personnelles de R&D, pas des missions clients.** Chaque étude de cas distingue l'architecture cible, le code présent, les résultats vérifiés et les limites encore ouvertes.

### 1. [MUTYVA — Applications natives déclaratives](https://github.com/cybou-fr/mutyva)
**C++20 · Qt 6.12 / QML · SQLite · Ingénierie assistée par IA**

Concevoir une application locale dont l'interface peut évoluer à partir de propositions d'IA **sans exécuter de code généré** et sans effacer les données utilisateur. Architecture modulaire, schémas contrôlés, générations immuables, transactions et décisions ADR.

- [Étude de cas (FR)](https://github.com/cybou-fr/mutyva/blob/main/docs/CASE_STUDY_FR.md)
- [Architecture, exigences et risques](https://github.com/cybou-fr/mutyva/blob/main/docs/23_ARCHITECTURE_ASSESSMENT.md)

*Statut : prototype en développement. Validation statique des contrats disponible ; qualification native Qt 6.12 encore à terminer.*

### 2. [CYBOU Browser — Navigateur natif et sécurité explicite](https://github.com/cybou-fr/CybouBrowser)
**C++20 · Qt WebEngine · QML · Threat modeling · Tests de sécurité**

Développer un navigateur desktop où les capacités demandées par les sites sont visibles et contrôlables. Séparation entre politique, demande observée, permission et usage effectif ; architecture par frontières de confiance ; validation de sécurité fondée sur des scénarios et des preuves.

- [Étude de cas (FR)](https://github.com/cybou-fr/CybouBrowser/blob/main/docs/CASE_STUDY_FR.md)
- [Qualité, preuves et limites](https://github.com/cybou-fr/CybouBrowser/blob/main/docs/ENGINEERING_QUALITY.md)

*Statut : 0.4.0-alpha.1, projet de développement ; aucune certification de sécurité ni version finale revendiquée.*

### 3. [ZFSCloud — Système de sauvegarde client–serveur](https://github.com/cybou-fr/zfscloud)
**Go · gRPC / Protobuf · Linux / ZFS · TLS/mTLS · Client GUI/CLI**

Assembler des services réseau, des contrats RPC, du stockage ZFS, des snapshots et plusieurs interfaces clientes. Le cas illustre l'intégration backend, infrastructure, protocole, sécurité et ergonomie.

- [Étude de cas (FR)](https://github.com/cybou-fr/zfscloud/blob/main/docs/CASE_STUDY_FR.md)

*Statut : sources et scénarios de test disponibles ; audit externe et cycle de vie des secrets à qualifier avant toute promesse de production.*

### 4. [ConfidIS OS — Stockage chiffré et fédération de nœuds](https://github.com/cybou-fr/ConfidIS)
**Rust · Systèmes distribués · Erasure coding · Cryptographie · Politiques de placement**

Concevoir une infrastructure auto-hébergée de traitement temporaire de données sensibles : chiffrement côté client, fragments Reed–Solomon, placement sur plusieurs nœuds et traçabilité d'exploitation.

- [Étude de cas (FR)](https://github.com/cybou-fr/ConfidIS/blob/main/docs/CASE_STUDY_FR.md)

*Statut : R&D en développement ; aucune certification réglementaire ou garantie de résilience terrain revendiquée.*

**Travaux complémentaires :** [Sodix — utilitaire CLI Rust / cryptographie](https://github.com/cybou-fr/sodix) et autres expérimentations accessibles dans les [dépôts publics](https://github.com/cybou-fr?tab=repositories).

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
