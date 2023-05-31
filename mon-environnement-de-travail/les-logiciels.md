---
description: Les outils utilisés
---

# Les Logiciels

### Confluence

Développé par l'éditeur de logiciel Australien Atlassian en 2004, Confluence est un logiciel de wiki, utilisé comme logiciel de travail collaboratif.

#### Travail de rédaction

Durant ce stage, j'ai été amené à rédiger des pages de documentation, autant pour avoir un suivi que pour détailler des procédures. Confluence est un logiciel de wiki, de travail collaboratif, et c'est ce qui est utilisé pour documenter des sujets. Les rédactions en question concernait les scripts Google Sheets, pour un suivi de l'avancement, des raisonnements, des évolutions et de la documentation, ainsi que des pages Confluence pour les demandes de droits (BDD Access, VMWARE, Confluences, Snow, Jira, etc...) et les procédures de renouvellement de certificats.

<figure><img src="../.gitbook/assets/confluence.png" alt=""><figcaption><p>Une page Confluence de certificat</p></figcaption></figure>

### Jira

Jira est un système de suivi de bugs et de gestion des incidents développé par Atlassian en 2002. Il nous permet des gérer les flux de tickets entrant.

<figure><img src="../.gitbook/assets/jira.png" alt=""><figcaption><p>Page Jira pour le suivi de mes tickets</p></figcaption></figure>

<figure><img src="../.gitbook/assets/process_jira_2.png" alt=""><figcaption></figcaption></figure>

Composition d'un ticket JIRA:

<figure><img src="../.gitbook/assets/details_ticket_jira.png" alt=""><figcaption></figcaption></figure>

* Son type : Incident, DIT AS, DIT MC (voir [Les Tickets](../ma-mission/les-tickets.md))
* Sa priorité : de 1 à 4, 1 étant le plus prioritaire
* Son état : Ouvert, Réalisation en Cours, Clos, En Attente, Déploiement en Cours (les états varient en fonction du ticket)
* Les Données générales et la Description qui donne des informations et le contexte
* Données complémentaire contient le lien du ticket sur SnowIT, le gestionnaire de ticket côté Suravenir

### Eclipse / IntelliJ

Eclipse est un environnement de production de logiciels, principalement en Java, dont la première version date de 2001.

<figure><img src="../.gitbook/assets/IntelliJ_IDEA_Icon.svg.png" alt="" width="188"><figcaption></figcaption></figure>

IntelliJ est un environnement de développement intégré (en anglais Integrated Development Environment ou IDE) destiné au développement de logiciels informatique Java. Conçu par JetBrain, la première version du framework est rendu publique en 2001.

Les développement se fond majoritairement via Eclipse, mais passerons progressivement sur IntelliJ, étant donné que les projets passerons sur Git à la place de SVN.

### Git / SVN

Subversion (ou SVN) est un logiciel de gestion de versions, distribué sous licence Apache3 et développé par Apache Software Fundation.

<div align="left">

<figure><img src="../.gitbook/assets/Apache_Subversion_logo.svg.png" alt="" width="135"><figcaption></figcaption></figure>

</div>

Subversion fonctionne sur le modèle client-serveur, avec :&#x20;

* un serveur centralisé et unique où se situent :
  * les fichiers constituant la référence (le "dépôt" ou "référentiel", "repository" en anglais),
  * un logiciel serveur Subversion tournant en tâche de fond;
* des postes clients sur lesquels se trouvent :&#x20;
  * les fichiers recopiés depuis le serveur, éventuellement modifiés localement depuis leur récupération,
  * un logiciel client, sous forme d'exécutable standalone (comme SmartSVN par exemple) ou de plug-in (Eclipse Subversive dans notre cas) permettant la synchronisation, manuelle et/ou automatisée, entre chaque client et le serveur de référence.

Git est un logiciel de gestion de versions décentralisé. C'est un logiciel libre et gratuit, créé en 2005 par Linus Torvalds, auteur du noyau Linux.

Depuis les années 2010, il s'agit du logiciel de gestion de versions le plus populaire dans le développement logiciel et web, qui est utilisé sur touts les environnements : Windws, Linux et Mac. Git est aussi le système à la base du site web GitHub, le plus important hébergeur de code informatique.

Les projets sont majoritairement sous SVN, mais migre progressivement vers Git.
