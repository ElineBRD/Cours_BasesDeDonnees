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
```

## Commandes pour manipuler les tables/colonnes

### Ajouter un objet

```sql
INSERT INTO nom_de_la_table (colonne1, colonne2, colonne3, ...)
VALUES (valeur1, valeur2, valeur3, ...);
```

### Créer une nouvelle table en ligne de commande
**Exemple** : créer une table appelée "cours" :
```sql
CREATE TABLE cours (
    id SERIAL PRIMARY KEY,
    matiere VARCHAR(100),
    jourHeure DATE,
    duree INT
);
```

### Ajouter, modifier et supprimer une colonne
```sql
ALTER TABLE eleve ADD (test integer)
ALTER TABLE eleve DROP (test)
ALTER TABLE eleve CHANGE
```

### Modifier des éléments


- Colonne :
    - RENAME TABLE [...] TO [...];
- Table :
    - ALTER TABLE
    - DROP TABLE
    - SHOW
    - CREATE TABLE
- DATABASE
    - USE
    - DROP
    - CREATE
- Donnée
    - INSERT
    - UPDATE
    - DELETE
    - SELECT