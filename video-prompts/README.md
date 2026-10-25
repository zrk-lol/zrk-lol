<div align="center">

<img src="../assets/divider.svg" width="100%" />

# 🎬 20 prompts vidéo pour Claude

**Copie un prompt, remplace ce qui est entre `[crochets]`, colle-le dans Claude Code : il te code la vidéo et te la rend en MP4.**

<a href="https://zrk.lol"><img src="https://img.shields.io/badge/par-%C8%A4rk-FF1E1E?style=for-the-badge&labelColor=0a0a0c" /></a>
<img src="https://img.shields.io/badge/prompts-20-FF1E1E?style=for-the-badge&labelColor=0a0a0c" />
<img src="https://img.shields.io/badge/moteur-Remotion-FF1E1E?style=for-the-badge&labelColor=0a0a0c" />
<a href="https://discord.gg/4qRhB4c5me"><img src="https://img.shields.io/badge/aide-Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white&labelColor=0a0a0c" /></a>

</div>

---

## ⚙️ Avant de commencer

1. Installe [Node.js](https://nodejs.org) (version 18 ou plus).
2. Ouvre un dossier vide dans **Claude Code** (terminal, app desktop ou VS Code).
3. Colle le prompt. Claude crée le projet [Remotion](https://www.remotion.dev), écrit les scènes et lance le rendu.
4. Ta vidéo sort dans `out/`. Pour la modifier, parle-lui normalement : « ralentis la 2ᵉ scène », « mets le logo plus gros ».

> 💡 Les images sont des **aperçus** : elles montrent l'idée générale, pas le rendu exact. Chaque vidéo sort un peu différente, c'est normal.
>
> 🎵 Pour la musique, mets un fichier `musique.mp3` dans `public/` avant de lancer le prompt, Claude l'ajoutera.

### Sommaire

| | | | |
|:-:|:-:|:-:|:-:|
| [01 · Intro néon](#01--intro-logo-néon) | [02 · Promo site](#02--promo-de-site-web) | [03 · App mobile](#03--démo-dapp-mobile) | [04 · Bot Discord](#04--bot-discord-en-action) |
| [05 · Glitch cyber](#05--glitch-cybersécurité) | [06 · Typo cinétique](#06--typographie-cinétique) | [07 · Halloween](#07--promo-halloween-10-) | [08 · Avis client](#08--avis-client-animé) |
| [09 · Chiffres clés](#09--chiffres-clés-animés) | [10 · Avant / Après](#10--avant--après) | [11 · Story Insta](#11--story-instagram) | [12 · Intro YouTube](#12--intro-de-chaîne-youtube) |
| [13 · Tuto terminal](#13--tuto-code-en-terminal) | [14 · Hosting](#14--lancement-dun-hébergement) | [15 · 3 étapes](#15--méthode-en-3-étapes) | [16 · Portfolio 3D](#16--showcase-portfolio-3d) |
| [17 · Particules](#17--logo-en-particules) | [18 · Offres](#18--offres-et-tarifs) | [19 · Sous-titres](#19--face-caméra-sous-titré) | [20 · Outro Discord](#20--outro--rejoins-le-discord) |

---

## 01 · Intro logo néon

<img src="previews/01.svg" width="100%" />

**Pour :** le début de tes vidéos, un logo qui s'allume comme une enseigne. 8 s, 16:9.

```text
Crée une vidéo avec Remotion (React + TypeScript) dans ce dossier. Installe ce qu'il faut, puis rends le MP4 dans out/intro-neon.mp4.

Format : 1920x1080, 30 fps, 8 secondes.
Couleurs : fond #0A0A0C, néon [#FF1E1E], texte secondaire #9A9AA4.

Scènes :
1. 0–1,5 s : écran noir, une grille rouge très discrète apparaît en fondu.
2. 1,5–4 s : le texte "[TON NOM OU LOGO]" s'allume lettre par lettre comme un néon (contour seulement, glow avec plusieurs drop-shadow). Deux ou trois grésillements d'opacité avant de rester allumé.
3. 4–6 s : sous le logo, "[TON SOUS-TITRE]" apparaît avec un letter-spacing qui se resserre.
4. 6–8 s : léger zoom avant (scale 1 → 1,06) et fondu au noir.

Contraintes : animations avec spring() et interpolate(), pas de librairie d'animation externe. Si public/musique.mp3 existe, ajoute-la avec un fade out sur la dernière seconde. À la fin, donne-moi la commande pour relancer le rendu.
```

---

## 02 · Promo de site web

<img src="previews/02.svg" width="100%" />

**Pour :** présenter un site que tu viens de livrer, avec une fausse fenêtre de navigateur qui défile. 20 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu final dans out/promo-site.mp4.

Format : 1920x1080, 30 fps, 20 secondes.
Site présenté : [NOM DU SITE] — [URL]. Couleur principale : [#FF1E1E]. Fond : #0A0A0C.

Mets ces captures dans public/ : [capture-accueil.png], [capture-page2.png], [capture-mobile.png]. Si elles n'existent pas, dessine des maquettes simples en CSS à la place.

Scènes :
1. 0–3 s : titre "[ACCROCHE COURTE, ex. Le nouveau site de Léa est en ligne]" qui monte depuis le bas.
2. 3–10 s : une fenêtre de navigateur (barre avec 3 points et l'URL) apparaît avec un spring. La capture d'accueil défile doucement vers le bas. Un curseur de souris se déplace et clique sur un bouton (petit effet de pression).
3. 10–15 s : la fenêtre se réduit à gauche, un téléphone apparaît à droite avec la capture mobile.
4. 15–20 s : écran final avec l'URL en gros, "[TON NOM] — création de sites" en dessous, fondu au noir.

Écris chaque scène dans son propre composant. Pas de texte en dehors de ce que je t'ai donné.
```

---

## 03 · Démo d'app mobile

<img src="previews/03.svg" width="100%" />

**Pour :** montrer une app iOS/Android en vertical, avec des cartes qui flottent autour du téléphone. 15 s, 9:16.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/demo-app.mp4.

Format : 1080x1920 (vertical), 30 fps, 15 secondes.
App : [NOM DE L'APP], elle sert à [CE QUE FAIT L'APP EN UNE PHRASE]. Couleur : [#FF1E1E], fond #0A0A0C.

Dessine un téléphone en CSS (coins arrondis, encoche). Dans l'écran, recrée 3 écrans de l'app en CSS : [ÉCRAN 1 : accueil avec ...], [ÉCRAN 2 : ...], [ÉCRAN 3 : ...].

Déroulé :
1. 0–2 s : le téléphone arrive du bas avec un spring, légèrement incliné, puis se redresse.
2. 2–11 s : on passe d'un écran à l'autre par un glissement horizontal, toutes les 3 s. À chaque écran, une carte de notification flotte à côté du téléphone (ex. "[Commande validée]", "[+38 % de ventes]").
3. 11–15 s : le téléphone recule, le nom de l'app et "[Disponible sur iOS et Android]" apparaissent dessous.

Garde un mouvement de flottement très léger sur les cartes (sinus sur translateY, 6 px max).
```

---

## 04 · Bot Discord en action

<img src="previews/04.svg" width="100%" />

**Pour :** faire la démo d'un bot Discord sans filmer ton écran. 20 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/demo-bot.mp4.

Format : 1920x1080, 30 fps, 20 secondes.
Bot : [NOM DU BOT]. Il fait : [FONCTION, ex. créer des tickets de support].

Recrée une interface façon Discord en CSS (thème sombre : #1E1F24, #2B2D31, liste de salons à gauche). Ne copie pas le logo Discord.

Déroulé :
1. 0–3 s : l'interface apparaît, le salon "#[NOM DU SALON]" est sélectionné.
2. 3–7 s : un membre "[PSEUDO]" tape la commande "[/commande argument]" caractère par caractère, puis l'envoie.
3. 7–9 s : indicateur "[NOM DU BOT] est en train d'écrire…".
4. 9–15 s : le bot répond avec un embed (bordure gauche [#FF1E1E], titre "[TITRE DE LA RÉPONSE]", texte "[DÉTAIL]", deux boutons "[BOUTON 1]" et "[BOUTON 2]"). Un curseur clique sur le premier bouton.
5. 15–20 s : zoom sur l'embed, puis carton final "[NOM DU BOT] — ajoute-le sur ton serveur".

Le texte tapé doit avoir une vitesse irrégulière, comme une vraie frappe.
```

---

## 05 · Glitch cybersécurité

<img src="previews/05.svg" width="100%" />

**Pour :** un teaser court et nerveux sur la sécurité, un audit ou un pentest. 10 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/glitch-cyber.mp4.

Format : 1920x1080, 30 fps, 10 secondes. Fond noir, police monospace.

Déroulé :
1. 0–3 s : un terminal affiche des lignes qui défilent vite : "> scan --target [TON-DOMAINE]", "ports...", "headers...", "ssl...". Chaque ligne finit par "OK" en vert #2EE66B.
2. 3–6 s : gros texte "[ACCESS GRANTED]" au centre avec un effet glitch : trois couches (cyan #00E5FF, rouge [#FF1E1E], blanc) décalées de quelques pixels, des bandes horizontales qui découpent le texte toutes les 4 à 6 images, et des scanlines.
3. 6–8 s : le glitch se calme, un cadenas dessiné en SVG se ferme.
4. 8–10 s : "[TON NOM] — [audit de sécurité / protection de ton site]" et ton URL.

Le glitch doit être déterministe (utilise random() de Remotion avec une seed), pour que le rendu soit identique à chaque fois.
```

---

## 06 · Typographie cinétique

<img src="previews/06.svg" width="100%" />

**Pour :** un message fort en quelques mots, sans images. 12 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/typo.mp4.

Format : 1920x1080, 30 fps, 12 secondes. Fond #0A0A0C, texte blanc, accent [#FF1E1E].
Police : [Inter / Archivo Black / autre Google Font], chargée avec @remotion/google-fonts.

Texte, une ligne à la fois :
"[UNE IDÉE.]"
"[DU CODE.]"
"[EN LIGNE.]"
"[TON NOM OU TON URL]"

Règles :
- Chaque mot arrive différemment : un qui tombe du haut, un qui sort d'un bloc de couleur qui se déroule derrière lui (légèrement penché, -3°), un qui s'écrit lettre par lettre.
- Les lignes précédentes restent à l'écran en gris, puis disparaissent quand la dernière arrive.
- Coupes franches, rythme calé sur 120 BPM (un temps = 15 images).
- Si public/musique.mp3 existe, ajoute-la.
```

---

## 07 · Promo Halloween −10 %

<img src="previews/07.svg" width="100%" />

**Pour :** une promo saisonnière avec un code et un compte à rebours. 15 s, carré 1:1 (Insta, Discord).

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/promo.mp4.

Format : 1080x1080, 30 fps, 15 secondes.
Offre : "[−10 %]" sur "[tous les services]" avec le code "[HALOWEEN26]", valable jusqu'au [DATE].
Ambiance : [Halloween — orange #FF7A18, noir, violet foncé] (change pour Noël, Black Friday, etc.).

Déroulé :
1. 0–3 s : des chauves-souris en SVG traversent l'écran, une citrouille dessinée en SVG apparaît avec un rebond.
2. 3–7 s : "[−10 %]" en très gros avec un glow, qui pulse une fois.
3. 7–11 s : le code promo dans un cadre en pointillés, comme un coupon. Il "se copie" : petite animation de clic et le texte "Copié" apparaît.
4. 11–15 s : compte à rebours jours/heures/minutes/secondes (les chiffres défilent vers le haut), puis "[TON URL]".

Dessine tout en SVG ou en CSS, sans image externe.
```

---

## 08 · Avis client animé

<img src="previews/08.svg" width="100%" />

**Pour :** transformer un vrai avis client en contenu pour les réseaux. 12 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/avis.mp4.

Format : 1920x1080, 30 fps, 12 secondes. Fond #0A0A0C, carte #121216, accent [#FF1E1E].

Avis (garde le texte exact, ne le reformule pas) :
"[COLLE ICI L'AVIS DU CLIENT]"
— [PRÉNOM N.], [MÉTIER OU ENTREPRISE]
Note : [5]/5

Déroulé :
1. 0–2 s : la carte arrive avec un spring et une ombre douce. Un gros guillemet rouge apparaît en haut à gauche.
2. 2–8 s : le texte de l'avis s'affiche mot par mot (pas lettre par lettre), au rythme d'une lecture normale.
3. 8–10 s : les étoiles se remplissent une par une, avatar rond avec l'initiale et le nom en dessous.
4. 10–12 s : la carte se décale à gauche, "[TON NOM] — [CE QUE TU FAIS]" apparaît à droite.

Si l'avis est long, réduis la taille du texte pour qu'il tienne en 4 lignes maximum.
```

---

## 09 · Chiffres clés animés

<img src="previews/09.svg" width="100%" />

**Pour :** montrer des résultats avec des compteurs et un graphique qui monte. 15 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/chiffres.mp4.

Format : 1920x1080, 30 fps, 15 secondes. Fond #0A0A0C, accent [#FF1E1E].

Chiffres (uniquement ceux-là, n'en invente pas) :
- [+120 %] — [de visites en 3 mois]
- [48 h] — [pour la première maquette]
- [30] — [projets livrés]

Données du graphique (5 barres) : [50, 80, 70, 120, 165], étiquettes : [Juin, Juil, Août, Sept, Oct].

Déroulé :
1. 0–6 s : chaque chiffre compte de 0 à sa valeur en 1,5 s (easing out), avec sa légende qui apparaît en dessous.
2. 6–12 s : à droite, les barres montent l'une après l'autre, puis une courbe blanche se dessine par-dessus (stroke-dashoffset). Petite étiquette "[record]" sur la dernière barre.
3. 12–15 s : "[TON NOM]" et ton URL.

Utilise des nombres formatés en français (espace pour les milliers, virgule pour les décimales).
```

---

## 10 · Avant / Après

<img src="previews/10.svg" width="100%" />

**Pour :** montrer une refonte de site avec un curseur qui glisse entre l'ancien et le nouveau. 12 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/avant-apres.mp4.

Format : 1920x1080, 30 fps, 12 secondes.
Mets dans public/ : [avant.png] (ancien site) et [apres.png] (nouveau site), même taille.

Déroulé :
1. 0–2 s : l'image "avant" seule, étiquette "AVANT" en haut à gauche.
2. 2–8 s : une ligne verticale blanche avec une poignée ronde glisse de gauche à droite et révèle "après" (clip-path). Elle s'arrête au milieu, repart un peu en arrière, puis va jusqu'au bout. Étiquette "APRÈS" en [#FF1E1E].
3. 8–12 s : l'image "après" en plein écran avec un léger zoom, puis "[NOM DU CLIENT] — refonte par [TON NOM]".

Le mouvement de la poignée doit ressembler à quelqu'un qui la tire à la main (accélérations et ralentissements), pas à un glissement linéaire.
```

---

## 11 · Story Instagram

<img src="previews/11.svg" width="100%" />

**Pour :** annoncer un lancement en story, avec stickers et sondage. 15 s, 9:16.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/story.mp4.

Format : 1080x1920, 30 fps, 15 secondes (3 slides de 5 s).
Compte : [@TONCOMPTE]. Couleur : [#FF1E1E].

Recrée l'interface d'une story : barres de progression en haut qui se remplissent, photo de profil ronde et nom du compte.

Slides :
1. Fond dégradé, sticker penché "[NOUVEAU SITE]" qui arrive avec un rebond, puis une capture [public/site.png] dans un cadre de navigateur.
2. Trois points forts du projet, un par un : "[POINT 1]", "[POINT 2]", "[POINT 3]".
3. Sticker sondage "[Tu valides ?]" avec deux réponses "[OUI]" / "[GRAVE]". Un doigt (cercle semi-transparent) tape sur une réponse, les pourcentages s'affichent.

Laisse 250 px de marge en haut et en bas pour que rien ne passe sous l'interface d'Instagram.
```

---

## 12 · Intro de chaîne YouTube

<img src="previews/12.svg" width="100%" />

**Pour :** les 5 premières secondes de tes vidéos YouTube, avec le bouton s'abonner. 6 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/intro-yt.mp4, plus une version avec fond transparent en out/intro-yt.mov (codec ProRes 4444).

Format : 1920x1080, 30 fps, 6 secondes.
Chaîne : [NOM DE LA CHAÎNE], phrase : "[CE QU'ON TROUVE SUR LA CHAÎNE]". Couleur : [#FF1E1E].

Déroulé :
1. 0–1,5 s : un cercle avec l'initiale "[Z]" se dessine (stroke-dashoffset) puis se remplit.
2. 1,5–3 s : le nom de la chaîne glisse depuis le cercle vers la droite, la phrase apparaît dessous.
3. 3–5 s : un bouton "S'ABONNER" rouge, un curseur arrive et clique. Le bouton devient gris "ABONNÉ" et une cloche dessinée en SVG se balance.
4. 5–6 s : tout se replie vers le cercle et disparaît.

Pour la version transparente, ne mets aucun fond.
```

---

## 13 · Tuto code en terminal

<img src="previews/13.svg" width="100%" />

**Pour :** expliquer une commande ou un setup, sans enregistrer ton écran. 30 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/tuto.mp4.

Format : 1920x1080, 30 fps, 30 secondes.
Sujet : [CE QUE LE TUTO MONTRE, ex. créer un bot Discord en 3 commandes].

Commandes et sorties à afficher (garde-les exactes) :
$ [COMMANDE 1]
[SORTIE 1]
$ [COMMANDE 2]
[SORTIE 2]
$ [COMMANDE 3]
[SORTIE 3]

Rendu :
- Une fenêtre de terminal macOS en CSS (3 points, titre "[zsh — ~/projet]"), fond #0D0D10, police JetBrains Mono via @remotion/google-fonts.
- Les commandes se tapent à vitesse humaine, les sorties apparaissent d'un coup. Les lignes qui commencent par ✔ sont en vert, les erreurs en [#FF1E1E].
- Curseur bloc qui clignote.
- Une barre de progression pour la dernière commande.
- En bas à droite, une étiquette qui indique l'étape : "Étape 1/3", etc.
- Fin : "[TON NOM] — plus de tutos sur [URL]".
```

---

## 14 · Lancement d'un hébergement

<img src="previews/14.svg" width="100%" />

**Pour :** teaser un produit ou un service qui arrive, avec un faux panel d'admin. 20 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/teaser-hosting.mp4.

Format : 1920x1080, 30 fps, 20 secondes.
Produit : [Ȥrk. Hosting] — [héberge tes bots Discord et tes sites, gérés depuis un panel web]. Sortie : [BIENTÔT / DATE].

Déroulé :
1. 0–4 s : noir, un curseur clignote, la phrase "[Ton bot plante à 3 h du matin ?]" se tape.
2. 4–12 s : un panel d'admin apparaît (CSS) : menu à gauche, liste de services avec un point de statut ("[bot-musique] en ligne", "[site-client] en ligne", "[bot-tickets] redémarrage"), un graphique CPU qui bouge en temps réel. Le statut orange passe au vert.
3. 12–16 s : trois arguments, un par un : "[ARGUMENT 1]", "[ARGUMENT 2]", "[ARGUMENT 3]".
4. 16–20 s : tampon "COMING SOON" qui s'écrase sur l'écran (scale 3 → 1, léger tremblement), puis "[URL]".

N'invente pas de prix ni de caractéristiques techniques.
```

---

## 15 · Méthode en 3 étapes

<img src="previews/15.svg" width="100%" />

**Pour :** expliquer comment tu travailles avec un client. 15 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/methode.mp4.

Format : 1920x1080, 30 fps, 15 secondes. Fond #0A0A0C, accent [#FF1E1E].

Étapes :
01 — [On discute] — [ton idée, tes objectifs, ton budget]
02 — [Je construis] — [design, développement et tests avec toi]
03 — [Je t'accompagne] — [mise en ligne et suivi après livraison]

Déroulé :
1. 0–2 s : titre "[DE L'IDÉE À LA MISE EN LIGNE]" en petites capitales espacées.
2. 2–13 s : une ligne horizontale se dessine de gauche à droite. Quand elle atteint chaque étape, le cercle se remplit de rouge, le numéro apparaît et le texte monte en dessous. Un point lumineux suit le bout de la ligne.
3. 13–15 s : "[TON URL]".

Chaque étape doit rester lisible au moins 3 secondes.
```

---

## 16 · Showcase portfolio 3D

<img src="previews/16.svg" width="100%" />

**Pour :** faire défiler tes projets en cartes inclinées, effet carrousel. 20 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/portfolio.mp4.

Format : 1920x1080, 30 fps, 20 secondes.
Projets (mets les captures dans public/) :
1. [NOM PROJET 1] — [type, ex. site vitrine] — public/[p1.png]
2. [NOM PROJET 2] — [type] — public/[p2.png]
3. [NOM PROJET 3] — [type] — public/[p3.png]
4. [NOM PROJET 4] — [type] — public/[p4.png]

Rendu :
- Les cartes sont en carrousel 3D (CSS perspective + rotateY). La carte du centre est droite et nette, celles des côtés sont tournées à ±25°, plus petites et un peu sombres.
- Toutes les 4 s, le carrousel tourne d'un cran (spring, sans rebond excessif). Le nom et le type du projet central s'affichent en dessous.
- Reflet léger sous les cartes (copie retournée avec un dégradé de transparence).
- Fin : "[TON NOM] — portfolio complet sur [URL]".
```

---

## 17 · Logo en particules

<img src="previews/17.svg" width="100%" />

**Pour :** une révélation de logo qui se forme à partir de points. 8 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/particules.mp4.

Format : 1920x1080, 30 fps, 8 secondes. Fond #050506, particules [#FF4D4D] et blanches.

Logo : le texte "[ZRK]" (ou le fichier public/[logo.svg] s'il existe).

Méthode :
- Échantillonne la forme du logo (dessine-le dans un canvas hors écran et récupère environ 1 500 points sur les pixels pleins).
- Chaque particule part d'une position aléatoire (seed fixe avec random() de Remotion).

Déroulé :
1. 0–2 s : particules qui dérivent lentement, comme de la poussière.
2. 2–5 s : elles convergent vers leur place dans le logo, chacune avec un petit délai différent.
3. 5–6,5 s : le logo est formé, il pulse une fois avec un glow.
4. 6,5–8 s : "[TON SOUS-TITRE]" apparaît dessous, fondu au noir.

Rends les particules dans un seul <canvas>, pas en éléments DOM, pour que le rendu reste rapide.
```

---

## 18 · Offres et tarifs

<img src="previews/18.svg" width="100%" />

**Pour :** présenter tes offres en 3 cartes, avec celle du milieu mise en avant. 15 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/offres.mp4.

Format : 1920x1080, 30 fps, 15 secondes. Fond #0A0A0C, cartes #121216, accent [#FF1E1E].

Offres (texte exact, n'ajoute rien) :
1. [Vitrine] — [prix ou "Sur devis"] — [point 1] / [point 2] / [point 3]
2. [Boutique] — [prix ou "Sur devis"] — [point 1] / [point 2] / [point 3] — badge "[LE PLUS DEMANDÉ]"
3. [Sur mesure] — [prix ou "Sur devis"] — [point 1] / [point 2] / [point 3]

Déroulé :
1. 0–2 s : titre "[MES OFFRES]".
2. 2–8 s : les trois cartes montent l'une après l'autre. Dans chaque carte, les points apparaissent avec une coche qui se dessine.
3. 8–11 s : la carte du milieu grossit un peu, sa bordure devient rouge et le badge tombe dessus.
4. 11–15 s : bouton "[Demander un devis]" sur chaque carte, puis "[URL]".
```

---

## 19 · Face caméra sous-titré

<img src="previews/19.svg" width="100%" />

**Pour :** ajouter des sous-titres dynamiques (mot par mot, mot clé surligné) à une vidéo où tu parles. 30 s, 9:16.

```text
Crée un projet Remotion (React + TypeScript) qui ajoute des sous-titres animés à ma vidéo. Rendu dans out/sous-titres.mp4.

Vidéo source : public/[face-cam.mp4] (vertical 1080x1920).
Transcription : utilise @remotion/install-whisper-cpp pour transcrire la vidéo en [français] avec les timings par mot. Si ça ne marche pas, demande-moi le texte.

Style des sous-titres :
- 2 à 4 mots affichés à la fois, centrés à 70 % de la hauteur.
- Police [Montserrat Black], majuscules, blanc avec contour noir.
- Le mot prononcé à l'instant grossit légèrement (scale 1,1) et passe en [jaune #FFD23F].
- Ces mots-clés ont un fond coloré derrière : [SITE], [APP], [BOT], [GRATUIT].

Ajoute aussi un point rouge "REC" qui clignote en haut à gauche, et une barre de progression fine en bas.
```

---

## 20 · Outro : rejoins le Discord

<img src="previews/20.svg" width="100%" />

**Pour :** la fin de tes vidéos, pour envoyer les gens sur ton serveur. 8 s, 16:9.

```text
Crée une vidéo Remotion (React + TypeScript), rendu dans out/outro.mp4.

Format : 1920x1080, 30 fps, 8 secondes. Fond #0A0A0C.
Serveur : [NOM DU SERVEUR], lien : [discord.gg/4qRhB4c5me]. Site : [zrk.lol].

Déroulé :
1. 0–2 s : une icône de bulle de chat en SVG (pas le logo officiel Discord) s'allume en néon violet #7C86FF.
2. 2–4 s : "[Rejoins le serveur]" en gros, puis "[CE QU'ON Y TROUVE, ex. projets, entraide et coulisses]".
3. 4–6,5 s : le lien dans un bouton #5865F2 qui pulse doucement, et un compteur de membres qui monte jusqu'à "[NOMBRE] membres" (supprime cette partie si je n'ai pas mis de nombre).
4. 6,5–8 s : l'URL du site en petit, fondu au noir.

Laisse les 2 dernières secondes assez calmes pour que YouTube puisse y placer ses écrans de fin.
```

---

<div align="center">

**Tu as fait une vidéo avec un de ces prompts ?** Montre-la sur le [Discord](https://discord.gg/4qRhB4c5me) 👀

[← Retour au profil](https://github.com/zrk-lol) · [zrk.lol](https://zrk.lol)

<img src="../assets/divider.svg" width="100%" />

</div>
