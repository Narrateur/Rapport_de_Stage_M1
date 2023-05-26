# Les Tickets

Durant l'autre partie du stage, j'ai du apprendre à prendre en charge des tickets. Ici, ont en distingue 3 types:

* DIT MC : demande d'intervention technique à une TMA, de type maintenance corrective
* DIT AS : demande d'intervention technique à une TMA, de type assistance/support (ex: édition, les doc qui remonte pas dans la validation)
* incident : dysfonctionnement entrainant l'interruption ou la dégradation d'un service (ex: certificats)

La TMA doit aussi géré des tickets:

* certificats (renouvellement de certificats ssl bientôt expiré sur les différents projets)
* Edition batch (documents qui ne remonte pas dans oriadys -> problème lié à son nom -> l'édition et la confirmation n'ont pas le meme nom (c'est l'édition le pb son timestamp n'est pas le même que celui de la confirmation dans la bdd))
* edition (rejouer une requete soap. ex: rejouer une requête SOAP afin de re-générer un justificatif)
* recherche de logs (Une erreur s'affiche lorsque l'utilisateur manipule l'application -> chercher dans les logs l'erreur qui est survenu et en déduire la cause)
* purge de rejets (qué cé c'est?)

### Incident

Les incidents sont des dysfonctionnement entraînant l'interruption ou la dégradation d'un service. Il peut s'agir d'une erreur remonté par un utilisateur ou de certificats qui seront bientôt expiré.

### Demande d'Intervention Technique à une TMA, de type Assistance/Support (DIT AS)

Ces demandes indiquent que le problème ne bloque pas l'utilisation de l'application. Ce type de ticket peut faire référence à des documents qui n'apparaissent pas sur le site par exemple.

### Demande d'Intervention Technique à une TMA, de type Maintenance Corrective (DIT MC)

Ces demande indiquent que le problème doit être résolue via du développement. Une fonctionnalité indisponible, une évolution ou encore des tickets fréquent de cause similaire peuvent en être la source.

### Les Certificats

Les certificats SSL permettent aux sites web de passer de HTTP à HTTPS, ce qui est plus sécurisé. Un certificats SSL est un fichier de données hébergé dans le serveur d'origine d'un site Web. Les certificats SSL rendent le chiffrement SSL/TLS possible. Ils contiennent la clé publique du site, l'identité du site web ainsi que des informations connexes. Les appareils qui tentent de communiquer avec le serveur référencerons ce fichier pour obtenir la clé publique et vérifier l'identité du serveur. La clé privé est gardée secrète et sécurisée.

SSL (Secure Socket Layer), plus communément appelé TLS (Transport Layer Security) esy un protocole de chiffrement du trafic Internet et de vérification de l'identité des serveurs. Tout site Web avec une adresse web HTTPS utilise SSL/TLS.

Un certificat SSL contient les informations suivantes:

* Un émetteur, qui indique quel Autorité de Certification a émis le certificats.
* L'identité dont le certificats apporte la preuve (un nom de domaine, une personne, une organisation, une machine, etc. pour lequel le certificat a été délivré)
* Une signature numérique de l'Autorité de Certification qui a émis le certificat
* Les dates de validité (émission / expiration)
* La clé publique du certificat

2 points à noter:

* le contenu d'un certificat est public, il n'y a rien à protéger.
* La clé privée prouve que le certificat nous appartient. Le couple {clé privé + certificat} correspond à une pièce d'identité, mais au format numérique. Perdre la clé privée revient à perdre sa pièce d'identité.

Les extensions de fichiers:

* Les Certificate Signing Request (CSR) sont des ".csr"
* Les certificats sont généralementsont des ".crt"
* Les clé privé ".key"
* L'ensemble {certificat + clé privée}, qui sont normalement protégés par un mot de passe, sont des ".p12" (pour Linux)

Certificats Internes / Certificats Externes

* Les certificats internes : pour les sites privé, qui ne seront contactés que par des membres internes du Crédit mutuel Arkéa (CMA).
* Les certificats externes : pour les sites publiques, qui doivent être contactés par tous à travers le monde.

Les certificats traités dans notre cas sont essentiellement (voir exclusivement) des certificats client-interne. Ces certificats sont utilisés pour identifier un client ou un utilisateur, par son authentification auprès du serveur qui établit précisément qui il est.

Le renouvellement des certificats nécessite certaines procédures, qui peuvent changer d'un projet à l'autre. Il existe une page Confluence par certificats sous notre responsabilité. De cette manière, nous possédons à la fois un suivi sur l'état du renouvellement du certificats, mais aussi et surtout la procédure à effectuer pour renouveler ce certificats.
