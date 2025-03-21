# Bases de données : SQL

##

### Affichage de toute la table :

```sql
SELECT * FROM /* Une table */ ;
SELECT liste_des_attributs FROM une_table;
```

### Occurrence unique

```sql
SELECT DISTINCT /* ... */ FROM /* ... */;
SELECT DISTINCT NumIUT FROM Personne ;
```

### Clause WHERE
Utilisée pour filtrer les lignes d'une table de base de données en fonction d'une condition spécifiée.

```sql
SELECT * FROM Etudiant WHERE age > 25 AND ville IN ('Paris', 'Lyon', 'Londres');
SELECT * FROM Etudiant WHERE age > 25 OR ville IN ('Paris', 'Lyon', 'Londres');
SELECT * FROM WHERE age > 25 AND ville IN ('Paris', 'Lyon', 'Londres');
/* Trouver l'étudiant vivant en France à Brudges */
SELECT * FROM Etudiant WHERE pays = 'France' AND ville = 'Bruges';