# FCSC 2026 Spidersaurus

Suite à quelques déboires avec le langage [FORTH](https://hackropole.fr/fr/challenges/pwn/fcsc2023-pwn-may-the-forth/), ainsi que le langage [BASIC](https://hackropole.fr/fr/challenges/pwn/fcsc2025-pwn-back-to-basic/), notre développeur a décidé d’un retour aux origines de l’Internet Multimédia à l’aide de la [version 1.3](https://ftp.mozilla.org/pub/mozilla/source/mozilla-19980603.tar.gz) de l’interpréteur JavaScript SpiderMonkey.

Il nous assure qu’aucune faille de sécurité n’est exploitable, grâce aux paramètres de compilation ; de plus, il nous garantit que le code est certifié pour le passage à l’an 2000.

Cependant, un hacker anonyme nous a transmis un mystérieux fichier `test.js` qui semble déclencher une lecture de mémoire non initialisée. Pouvez-vous prouver que notre développeur a tort en lisant le contenu de la variable flag ?

**Note :** Le programme est compilé par `clang-17` (sous Debian 13 *i386*), mais s’exécute sous Debian 13 *amd64* (avec `libc6:i386` installé).

Auteur : cde

Origine : [Spidersaurus](https://hackropole.fr/fr/challenges/pwn/fcsc2026-pwn-spidersaurus/)


## Challenge
[files/JSRef.zip](files/JSRef.zip)
[files/spidersaurus](files/spidersaurus)
[files/spidersaurus.patch](files/spidersaurus.patch)

-----------

## Installation manuel
Vous n'utilisez pas l'application **les CTFs de Cyrhades** ? C'est dommage !
Mais voici comment installer ce CTF manuellement :

> git clone https://github.com/Hack-Oeil/fcsc2026-pwn-spidersaurus.git

> cd fcsc2026-pwn-spidersaurus

> docker compose -f docker-compose-default.yml up

-----------

## Sur le site officiel hackropole.fr
> https://hackropole.fr/fr/challenges/pwn/fcsc2026-pwn-spidersaurus/
