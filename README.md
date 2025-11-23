📘 Gestion des Comptes Bancaires — React + GraphQL + Spring Boot

Cette application permet de gérer des comptes bancaires via une interface web moderne construite avec React + Apollo Client, connectée à un backend Spring Boot GraphQL.

Elle propose trois grandes fonctionnalités :

Ajout de compte bancaire

Ajout de transaction (dépôt / retrait)

Affichage automatique des listes (comptes + transactions)

⚙️ Installation
🔹 1. Backend (Spring Boot)

Ouvrir le projet backend dans IntelliJ ou VS Code

Exécuter l’application :

mvn spring-boot:run


Accéder aux interfaces :

GraphQL : http://localhost:8082/graphql

H2 Console : http://localhost:8082/h2-console

Paramètres H2 :

Paramètre	Valeur
URL	jdbc:h2:mem:banque
User	sa
Password	(vide)
🔹 2. Frontend (React + Apollo Client)

Dans le dossier du projet frontend :

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

L’utilisateur peut créer un compte en saisissant :

un solde initial

un type de compte (COURANT ou EPARGNE)

Une fois validé :

le backend crée le compte

une date de création automatique est ajoutée

le compte apparaît instantanément dans la liste des comptes

✔️ 2. Affichage de la liste des comptes

L’application affiche automatiquement tous les comptes avec :

ID du compte

Solde

Type de compte

Date de création

La liste se met à jour en temps réel après chaque ajout.

✔️ 3. Ajout d’une transaction

L’utilisateur peut effectuer :

un dépôt

un retrait

Il doit renseigner :

l’ID du compte

le montant

le type de transaction

Après validation :

la transaction est enregistrée

une date automatique est ajoutée

✔️ 4. Affichage de la liste des transactions

La liste des transactions affiche :

Montant

Type (DEPOT ou RETRAIT)

Date

Compte associé

🖼️ Captures d’écran


https://github.com/user-attachments/assets/3e5e5daf-dd46-4295-8ae2-dfae9c7fbe61

