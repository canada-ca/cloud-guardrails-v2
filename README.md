# GC Cloud Guardrails – BETA

([Français](#mesures-de-protection-du-nuage-du-gouvernement-du-canada))

## Introduction

In August 2019, the Government of Canada (GC) established the [GC Cloud Guardrails](https://github.com/canada-ca/cloud-guardrails). The [GC Cloud Guardrails](https://github.com/canada-ca/cloud-guardrails) are mandated under the [Directive on Service and Digital](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32601) [Appendix G: Standard on Enterprise Information Technology Service Common Configurations](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32713). The [GC Cloud Guardrails](https://github.com/canada-ca/cloud-guardrails) are a preliminary set of baseline security controls to ensure that the cloud service environment has a minimum set of configurations for the cloud environment.

Currently, the guardrails are going through an update cycle. The updated version is presented as GC Cloud Guardrails – BETA in this repo.

## Purpose

To seek industry feedback on GC Cloud Guardrails – BETA.

## Questions

The following are questions for industry:

1. Do you have any comments on the proposed update to the cloud guardrails?
2. Do you anticipate any challenges for customers in implementing, validating, and reporting on compliance for the proposed guardrails?
3. For SaaS, what is the recommended approach for validating the guardrails either manually, or ideally in an automated manner?

## Definitions

For this document the following definitions will be used:

- Mandatory requirements: A set of baseline security controls that departments must implement, validate, and report on in the first 30 business days.
- Additional considerations: Additional security controls that are highly recommended and should be taken into consideration. While these are not expected to be implemented within 30 business days, they include best practices that should be considered as departments progress with the establishment of their cloud-based environments.

## Cloud Guardrails

| ID. | Cloud Guardrails                                                                      |
| --- | ------------------------------------------------------------------------------------- |
| 01  | [Protect User Accounts and Identities](EN/01_Protect-user-accounts-and-identities.md) |
| 02  | [Manage Access](EN/02_Manage-Access.md)                                               |
| 03  | [Secure Endpoints](EN/03_Secure-Endpoints.md)                                         |
| 04  | [Enterprise monitoring accounts](EN/04_Enterprise-Monitoring-Accounts.md)             |
| 05  | [Data location](EN/05_Data-Location.md)                                               |
| 06  | [Protection of data-at-rest](EN/06_Protect-Data-at-Rest.md)                           |
| 07  | [Protection of data-in-transit](EN/07_Protect-Data-in-Transit.md)                     |
| 08  | [Segment and separate](EN/08_Segmentation.md)                                         |
| 09  | [Network security services](EN/09_Network-Security-Services.md)                       |
| 10  | [Cyber defense services](EN/10_Cyber-Defense-Services.md)                             |
| 11  | [Logging and monitoring](EN/11_Logging-and-Monitoring.md)                             |
| 12  | [Configuration of cloud marketplaces](EN/12_Cloud-Marketplace-Config.md)              |
| 13  | [Plan for Continuity](EN/13_Plan-for-Continuity.md)                                   |

## How to Contribute

See [CONTRIBUTING.md](CONTRIBUTING.md)

## License

Unless otherwise noted, the source code of this project is covered under Crown Copyright, Government of Canada, and is distributed under the [MIT License](LICENSE).

The Canada wordmark and related graphics associated with this distribution are protected under trademark law and copyright law. No permission is granted to use them outside the parameters of the Government of Canada's corporate identity program. For more information, see [Federal identity requirements](https://www.canada.ca/en/treasury-board-secretariat/topics/government-communications/federal-identity-requirements.html).

---

<!-- markdownlint-disable MD024 MD025 -->

# Mesures de protection du nuage du gouvernement du Canada

<!-- ## Introduction

In August 2019, the Government of Canada (GC) established the [GC Cloud Guardrails](https://github.com/canada-ca/cloud-guardrails). The [GC Cloud Guardrails](https://github.com/canada-ca/cloud-guardrails) are mandated under the [Directive on Service and Digital](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32601) [Appendix G: Standard on Enterprise Information Technology Service Common Configurations](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32713). The [GC Cloud Guardrails](https://github.com/canada-ca/cloud-guardrails) are a preliminary set of baseline security controls to ensure that the cloud service environment has a minimum set of configurations for the cloud environment.

Currently, the guardrails are going through an update cycle. The updated version is presented as GC Cloud Guardrails – BETA in this repo.

## Purpose

To seek industry feedback on GC Cloud Guardrails – BETA.

## Questions

The following are questions for industry:

1. Do you have any comments on the proposed update to the cloud guardrails?
2. Do you anticipate any challenges for customers in implementing, validating, and reporting on compliance for the proposed guardrails?
3. For SaaS, what is the recommended approach for validating the guardrails either manually, or ideally in an automated manner?

## Definitions

Les définitions suivantes sont utilisées pour ce document :

- Exigences obligatoires : Un ensemble de mesures de sécurité de base que les ministères doivent mettre en œuvre, valider et faire rapport dans les 30 premiers jours ouvrables.
- Autres considérations : Autres mesures de sécurité qui sont fortement recommandées et doivent être prises en considération. Bien que l’on ne s’attende pas à ce qu’elles soient mises en œuvre dans les 30 jours ouvrables, elles comprennent les pratiques exemplaires qui devraient être prises en compte à mesure que les ministères progressent dans la mise en place de leur environnement en nuage. -->

## Mesures de protection du nuage

| ID. | Mesures de protection du nuage                                                                                        |
| --- | --------------------------------------------------------------------------------------------------------------------- |
| 01  | [Protéger les comptes d’utilisateurs et les identités](FR/01_Protéger-les-comptes-d’utilisateurs-et-les-identités.md) |
| 02  | [Gérer l’accès](FR/02_Gérer-l’accès.md)                                                                               |
| 03  | [Sécuriser les points d’extrémité](FR/03_Sécuriser-les-points-d’extrémité.md)                                         |
| 04  | [Comptes de surveillance de l’organisation](FR/04_Comptes-de-surveillance-de-l’organisation.md)                       |
| 05  | [Emplacement des données](FR/05_Emplacement-des-données.md)                                                           |
| 06  | [Protection des données inactives](FR/06_Protection-des-données-inactives.md)                                         |
| 07  | [Protection des données en transit](FR/07_Protection-des-données-en-transit.md)                                       |
| 08  | [Segmenter et séparer](FR/08_Segmenter-et-séparer.md)                                                                 |
| 09  | [Services de sécurité des réseaux](FR/09_Services-de-sécurité-des-réseaux.md)                                         |
| 10  | [Services de cyberdéfense](FR/10_Services-de-cyberdéfense.md)                                                         |
| 11  | [Enregistrement et surveillance](FR/11_Enregistrement-et-surveillance.md)                                             |
| 12  | [Configuration des marchés de l’informatique en nuage](FR/12_Configuration-des-marchés-de-l’informatique-en-nuage.md) |
| 13  | [Planifier la continuité](FR/13_Planifier-la-continuité.md)                                                           |

## Façon de contribuer

Consulter [CONTRIBUTING.md](CONTRIBUTING.md)

## Licence

Sauf indication contraire, le code source de ce projet est couvert par le droit d’auteur de la Couronne, gouvernement du Canada, et est distribué en vertu d’une [licence MIT](LICENSE).

Le mot-symbole Canada et les graphiques connexes liés à cette distribution sont protégés en vertu du droit des marques de commerce et des lois sur le droit d’auteur. Aucune permission n’est accordée pour les utiliser en dehors des paramètres du Programme de coordination de l’image de marque du gouvernement du Canada. Pour en apprendre davantage, consulter [Exigences pour l’image de marque](https://www.canada.ca/fr/secretariat-conseil-tresor/sujets/communications-gouvernementales/exigences-image-marque.html).
