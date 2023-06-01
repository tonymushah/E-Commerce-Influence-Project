# E-Commerce-Influence-Project (ECIP)

`Initially, a ITU project but a real later 😊`

## I - Specifications du projet

### Framework : [Remix](https://remix.run) (basee sur [Node.js](https://nodejs.org) et [React](https://react.dev))

### Framework UI : [Chakra UI](https://chakra-ui.com/)

### Package Manager : [PNPM](https://pnpm.io/)

### Base de donnee : [PostgreSQL](https://www.postgresql.org/)

### ORM (liaison entre front et back) : [Prisma](https://www.prisma.io/)

### Utilites : [Storybook](https://storybook.js.org/)

### Il est necessaire de comprendre avant tout React, Remix et Prisma avant de toucher au projet

## II - Mise en place local

0 - Installer [Node.js](https://nodejs.org) et [PNPM](https://pnpm.io/) (et [PostgreSQL](https://www.postgresql.org/))

Note : seuls les contributeurs peuvent contribuer au projet

1 - cloner le project localement avec

```bash
git clone https://github.com/tonymushah/E-Commerce-Influence-Project
```

2 - Puis ouvrir un terminal dans `website-fullstack` puis faite :

```bash
pnpm install
```

3 - creer une base de donnee de developpement dans POSTGRES :

### Recommendation :

Utiliser le script `db.test.sql`

4 - creer un fichier `.env` dans `website-fullstack` et ecrire :

```env
DATABASE_URL="postgresql://"nom_utilisateur":""@localhost:5432/base_de_donnee?schema=public"
```

5 - Deployment en local du serveur avec :

```bash
pnpm dev
```

## III - Conventions

### 1- Base de donnees

#### a - Modeles

Precede, par `MOD_`

Les modeles sont les tables de base qui vont etre les plus utilisee \
exemple : `MOD_Persone`, `MOD_Article`

#### b - Enumerution

Precede, par `ENUM_` \
Les donnees statiques commes le Sexe, disponibilite,...

exemple : `ENUM_Sexe`

#### c - Vues

Precede, par `V_`

#### d - Relation entre deux modeles

Precede, par `REL_` \
Une table qui va donc lien entre deux modeles \
Exemple : `REL_Olona_Article`,...

### 2 - Contribution 

#### Branche principale : `main`

Vous devez passer par un Pull request a chaque fois que vous faite un commit dans `main`

Votre `pull request` doit etre valide par le chef de projet technique

Vous pouver creer autant de branche que vous voulez mais il faut toujour passer par un `pull request` avant de le merge avec `main`

