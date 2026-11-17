# **Qu’est-ce qu’une table ?**<a href="../../"> <img src="../https://upload.wikimedia.org/wikipedia/commons/4/41/Microsoft_SQL_Server_2025_icon.svg" alt="SQL Server" align="right" height="64px"> </a>
En SGDBR c’est une relation ayant des relations avec d’autres table.  
Elle est constituer de lignes et colonnes. Une colonne est un attribut, et une ligne un upset.  
Chaque ligne reçoit un enregistrement de ligne.
```sql
/*************************
*  UTILISER LA BASE db   *
*************************/
USE [db] ; -- sans crochets sa fonctionne aussi

CREATE TABLE people (name VARCHAR(200) ) ;
CREATE TABLE peoples (name VARCHAR(200) , firstname VARCHAR(200) ) ;
```
## La modifer
Ca passe par la commande procédure stockée `Sp_rename`.
```sql
sp_rename 'people' , 'people1' ;
```
## La suppression
```sql
DROP TABLE people1 ;
```