# Database

### la base de donnée consiste à gerer un formation 

### la base de donnée n'est pas complet juste on à créer 4 tables pour faire de test sur les clés etrangeres
Tables_in_GestionFomation |
+---------------------------+
| assoEnFor                 |
| enseignant                |
| etudiant                  |
| formation                 |
| salle   

# prérequis pour utiliser ce programme 
    -installer mysql-server
    -se connecter sur le server mysql
    -tapez la commande suivant:
    
    // creation de base de donnée de nom gestion_Formation
    
          -create database gestion_Formation;
          
              
    // selectionner la base de donnée 
          -use gestion_Formation;
          
    // importation de nos tables avec les valeurs
          -source /chemin du base de donnée/nom De fichier.sql
          
    // verifiée si les tables sont deja importées
           -show tables;
                Tables_in_GestionFomation |
                 +---------------------------+
                 | assoEnFor                 |
                 | enseignant                |
                 | etudiant                  |
                 | formation                 |
                 | salle  
            
  //tapez la commande suivant     
 -select etudiant.*,formation.* from etudiant,formation where etudiant.id_for=formation.id_for;
              
              
+----+----------+-----------+--------+--------+--------+--------------------+
| id | nom      | prenom    | id_sal | id_for | id_for | libelle_for        |
+----+----------+-----------+--------+--------+--------+--------------------+
|  1 | Ingamar  | Biernat   |      2 |      2 |      2 | Sales              |
|  2 | Jocelin  | Duckerin  |      3 |      4 |      4 | Services           |
|  3 | Maurine  | Mackness  |      1 |      4 |      4 | Services           |
|  4 | Felipa   | Rudolph   |      2 |     10 |     10 | Product Management |
|  5 | Jule     | Stanmer   |      2 |      2 |      2 | Sales              |
|  6 | Nari     | Tunbridge |      2 |      2 |      2 | Sales              |
|  7 | Sheppard | Peers     |      2 |      2 |      2 | Sales              |
|  8 | Clement  | Wallworke |      4 |      4 |      4 | Services           |
|  9 | Gaspar   | Blackborn |      9 |      9 |      9 | Support            |
| 10 | Pattie   | Dennehy   |      1 |      1 |      1 | Engineering        |
+----+----------+-----------+--------+--------+--------+--------------------+
10 rows in set (0,00 sec)



#Félicitation

     
     
     
