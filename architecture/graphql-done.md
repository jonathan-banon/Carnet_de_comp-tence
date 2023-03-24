# GraphQL

> ❌ A travailler

> ✔️ Auto validation par l'étudiant

## 🎓 J'ai compris et je peux expliquer

- la différence entre REST et GraphQL ✔️
  
  - Le principal avantage de GraphQL est sa capacité à accéder à n’importe quel point de données ou à tous les points de données 
  via un point de terminaison d’API unique.

- les besoins auxquels répond GraphQL ✔️

    - Avec GraphQL, vous n’avez qu’un seul point de terminaison, vous n’avez donc pas besoin d’envoyer plusieurs requêtes pour récupérer différentes informations sur un objet

- la définition d'un schéma
- Query  ✔️

    - Discussion GraphQL permettant de consulter des données côté serveur ( requête GET  )

- Mutation  ✔️

    - Discussion GraphQL permettant de modifier des données côté serveur ( requête DELETE et POST  )

- Subscription ❌ / ✔️

    - Tout comme une 'Query' ,elle permet une consultation de données mais de façon plus durable. Elle permet de maintenir une connection active au serveur GraphQL ( Pratique pour notifier en temps réel des changements côté serveur )

## 💻 J'utilise

### Un exemple personnel commenté  ✔️
<!--
requête :
query GetPets {
    pets {
        name
    }
}

retour bdd :
{
    "data": {
        "pets": [
            {
                "name": "billy"
            },
            {
                "name": "bobby"
            }
        ]
    }
}
--->
### Utilisation dans un projet  ✔️

[lien github](https://github.com/WildCodeSchool/2022-11-turing-WildBlog/blob/dev/client/src/services/auth.query.ts)

Description :
Service d'authentification permettant de regrouper les requêtes qraphGL utilisées dans le projet
### Utilisation en production si applicable❌ / ✔️

[lien du projet](...)

Description :

### Utilisation en environement professionnel ❌ / ✔️

Description :

## 🌐 J'utilise des ressources


### Titre

 - https://graphql.org/learn/queries/
 - documentation GraphQL

 - https://www.apollographql.com/docs/apollo-server/
 - documentation serveur apollo


## 🚧 Je franchis les obstacles

### Point de blocage ❌ / ✔️

Description:

 - Utilisation graphQL dans un projet React avec serveur Apollo

Plan d'action : (à valider par le formateur)

- action 1   ❌ / ✔️
    - Configuration serveur apollo + graphQL côté serveur 
        - installation via gestionnaire de librairie :
            - apollo-serveur
            - graphQL
            - graphQL-scalars
            - typeorm
            - type-graphQL
    - Création fichier db.ts avec informations de connection pour la bdd
- action 2 ❌ / ✔️
    - Creation d'un shema
        <!--
            async function start(): Promise<void> {
                 schema = await buildSchema({
                resolvers: [UserResolver],
                : false,
                authChecker: customAuthChecker,
             });
        --->
    - Lancement du serveur Apollo
        <!--
            const server = new ApolloServer({
                schema,
                csrfPrevention: true,
                cache: "bounded",
                plugins: [ApolloServerPluginLandingPageLocalDefault({ embed: true })],
            })
        --->
    - Connection BDD
        <!--
            server.listen().then(async (data) => {
                await db.initialize();
                console.log(`server ready ${data.url}`);
            });
        --->
Résolution :

## 📽️ J'en fais la démonstration

- J'ai ecrit un [tutoriel](...) ❌ / ✔️
- J'ai fait une [présentation](...) ❌ / ✔️
