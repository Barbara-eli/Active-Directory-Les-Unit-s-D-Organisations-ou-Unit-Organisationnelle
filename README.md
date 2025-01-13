# Active-Directory-Les-Unit-s-D-Organisations-ou-Unit-Organisationnelle

Documentation : Création d'une Unité d'Organisation, d'un Groupe d'Utilisateurs et d'un Utilisateur dans Active Directory
*Prérequis* :
Il faut avoir accès à un serveur Windows avec Active Directory installé et configuré dans le domaine wilders.lan.
Vous devez avoir les droits d'administrateur ou des privilèges nécessaires pour gérer Active Directory.
*Objectifs* :
Créer une Unité d'Organisation (OU) Wilders_students.
Créer un Groupe d'utilisateurs Students dans cette OU.
Créer un utilisateur dans le groupe Students.
### Étape 1 : Créer une Unité d'Organisation Wilders_students
Ouvrir Active Directory Users and Computers sur le serveur où Active Directory est installé.
Dans le volet de gauche, faites un clic droit sur le domaine wilders.lan (ou le conteneur approprié) et sélectionner New > Organizational Unit.
Dans la fenêtre qui apparaît, entrer le nom de l'OU : **Wilders_students**.
Cliquer sur OK.
### Étape 2 : Créer un Groupe d'Utilisateurs Students
Dans Active Directory Users and Computers, localiser l'OU Wilders_students que vous venez de créer.
Faire un clic droit sur l'OU Wilders_students et sélectionnez New > Group.
Dans la fenêtre New Object – Group, entrer le nom du groupe : Students.
Laisser le champ Group Scope sur Global et le champ Group Type sur Security (cela permettra de gérer des permissions et d'ajouter des utilisateurs à ce groupe).
Cliquer sur OK pour créer le groupe Students.
### Étape 3 : Créer un Utilisateur dans le Groupe Students
Dans Active Directory Users and Computers, faire un clic droit sur l'OU Wilders_students et sélectionner New > User.

Dans la fenêtre New Object – User, entrer les informations pour le nouvel utilisateur (exemple : prénom John, nom de famille Doe).

First Name : John
Last Name : Doe
Full Name : John Doe
User logon name : jdoe
Cliquezrsur Next.

Définir un mot de passe pour l'utilisateur et choisir les options souhaitées (par exemple, User must change password at next logon si nécessaire).

Cliquer sur Next, puis sur Finish pour créer l'utilisateur.
### Étape 4 : Ajouter l'utilisateur au groupe Students
Toujours dans Active Directory Users and Computers, localisez l'utilisateur John Doe dans l'OU Wilders_students.
Faire un clic droit sur l'utilisateur et sélectionnez Add to a group....
Dans la fenêtre Enter the object names to select, taper Students et cliquer sur Check Names pour valider le groupe.
Cliquer sur OK pour ajouter l'utilisateur au groupe Students.
L'utilisateur John Doe est maintenant membre du groupe Students.
