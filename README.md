# SAÉ 2.4 · Auditer un environnement de test

> Projet intégratif de cybersécurité : audit d’un réseau de laboratoire, attaques contrôlées et failles web sur des applications volontairement vulnérables.

| | |
|---|---|
| **Formation** | BUT Réseaux et Télécommunications, Montbéliard |
| **Année** | 1<sup>re</sup> année, semestre 2 |
| **Organisation** | En équipe de 3 |
| **Outils et notions** | `Kali Linux` `Nmap` `Nessus` `Metasploit` `DVWA` `Injection SQL` `XSS` `Wireshark` `ESP8266` |

> Tous les tests ont été menés dans un **environnement de laboratoire isolé**, sur des machines prévues pour l’exercice.

## Partie cybersécurité

| Jalon | Travail |
|---|---|
| 1 | [Mise en place d’un serveur web sur ESP8266](cyber/jalons/jalon-01-serveur-esp8266.pdf) et vérification depuis Kali sur Raspberry Pi ([code](cyber/code/esp8266/esp8266.ino)) |
| 2 | [Inventaire des services du réseau avec Nmap](cyber/jalons/jalon-02-inventaire-nmap.pdf) ([tableau](cyber/jalons/jalon-02-inventaire-nmap.ods)) |
| 3 | [Analyse de vulnérabilités avec Nessus et recherche d’exploits Metasploit](cyber/jalons/jalon-03-nessus-metasploit.pdf) |
| 4 | [Attaques pratiques : déni de service, intrusion Samba, MITM](cyber/jalons/jalon-04-dos-samba-mitm.pdf) |
| 5 | [Injections SQL sur DVWA](cyber/jalons/jalon-05-injections-sql.pdf) |
| 6 | [XSS et récupération de cookies vers un serveur Flask](cyber/jalons/jalon-06-xss-vol-de-cookies.pdf) |

Le [rapport de cybersécurité](cyber/rapport-cybersecurite.pdf) reprend l’ensemble. Certaines tentatives n’ont pas abouti (par exemple, aucun exploit Metasploit trouvé pour le service DNS) : les comptes rendus le disent.

## Partie IOM (web)

Analyse d’une application PHP : lecture du code, récupération de mots de passe, observation d’une chaîne en clair dans Wireshark, faille XSS par l’URL puis sa correction. Les [captures d’écran](iom/captures/) sont numérotées dans l’ordre de la démarche.

## Contenu du dépôt

```
cyber/
  rapport-cybersecurite.pdf
  jalons/      comptes rendus des jalons 1 à 6
  code/        programme de l’ESP8266
  consignes/   fiches de TP et grille fournies par l’IUT
iom/
  captures/    captures de la partie web
  consignes/   fiches de TP fournies par l’IUT
```

Le code personnel d’activation Nessus a été retiré avant publication.

---

<sub>Bastien Lorenzi · BUT Réseaux et Télécommunications, parcours cybersécurité · [Portfolio](https://bastien-lorenzi.netlify.app/#projets) · [Profil GitHub](https://github.com/LORENZI-Bastien)</sub>
