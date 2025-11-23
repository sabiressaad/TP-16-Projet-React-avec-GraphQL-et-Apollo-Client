📘 Gestion des Comptes Bancaires — React + GraphQL + Spring Boot

Cette application permet de gérer des comptes bancaires à travers une interface web construite avec React, connectée à un backend Spring Boot GraphQL.
Elle couvre trois fonctionnalités principales : ajout de compte, ajout de transaction, et affichage des listes.

⚙️ Installation
🔹 1. Backend (Spring Boot)

Ouvrir le projet backend dans IntelliJ ou VS Code

Lancer l’application avec :

mvn spring-boot:run


Le backend tourne sur :

GraphQL : http://localhost:8082/graphql

H2 Console : http://localhost:8082/h2-console

URL : jdbc:h2:mem:banque

User : sa

Password : (vide)

🔹 2. Frontend (React + Apollo Client)

Dans le dossier du frontend :

npm install
npm start


Le frontend sera accessible sur :

👉 http://localhost:3000

📦 Dépendances principales
Backend

Spring Boot Web

Spring Boot GraphQL

Spring Data JPA

H2 Database

Lombok

Frontend

React

Apollo Client

GraphQL

TailwindCSS

🎯 Fonctionnalités de l’application
✔️ 1. Ajout d’un compte bancaire

L’utilisateur peut créer un nouveau compte en renseignant :

un solde initial

un type de compte (COURANT ou EPARGNE)

Une fois validé :

le backend crée le compte

une date de création automatique est ajoutée

le compte apparaît instantanément dans la liste

✔️ 2. Affichage de la liste des comptes

L’interface affiche tous les comptes enregistrés, avec :

ID du compte

Solde

Type de compte

Date de création

La liste se met à jour automatiquement à chaque ajout.

✔️ 3. Ajout d’une transaction

Il est possible d’effectuer :

un dépôt

un retrait

Pour chaque transaction, l’utilisateur saisit :

l’ID du compte concerné

le montant

le type de transaction

Une fois envoyée :

la transaction est enregistrée

une date automatique est ajoutée

✔️ 4. Affichage de la liste des transactions

Une section dédiée affiche toutes les transactions, avec :

Montant

Type (DEPOT ou RETRAIT)

Date

Compte associé

🖼️ Captures d’écran


https://github.com/user-attachments/assets/3e5e5daf-dd46-4295-8ae2-dfae9c7fbe61

