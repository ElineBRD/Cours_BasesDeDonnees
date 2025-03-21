# Exercices SQL

## Exercice 1 :
- Sélectionner le champ de tous les élèves
- Sélectionner **uniquement** les noms de tous les élèves
- Sélectionner l'adresse en la renommant "*email_professionnel*" et le nom et prenom de tous les élèves.
- Comment faire pour sélectionner tous les élèves par ordre de nom alphabétique ?

```sql
SELECT * FROM eleves;
SELECT names FROM eleves;
SELECT adresse_mail AS "email_professionnel", noms, prenoms FROM eleves; /* Renommer une colonne */
SELECT * FROM eleves ORDER BY noms ASC; /* Trier par odre alphabétique */
```

## Exercice 2 :

- Sélectionner toutes les informations de tous les élèves par **ordre alphabétique** du **nom**
- Sélectionner **uniquement** les noms de **tous les élèves**
- Sélectionner **uniquement** les noms **distincts** de **tous les élèves**
- Sélectionner les types étudiants distincts et par **ordre numérique**
- Sélectionner tous les élèves par odre alphabétique du nom et du prénom
- Sélectionner uniquement les adresses mails des élèves par ordre descendant.

```sql
SELECT * ORDER BY noms FROM eleves;
SELECT nom FROM eleves;
SELECT DISTINCT noms FROM eleves;
SELECT DISTINCT types_etudiants FROM eleve ORDER BY types_etudiants ASC;
SELECT * FROM eleves ORDER BY noms, prenoms ASC;
SELECT DISTINCT adresses_mail FROM eleve ORDER BY adresses_mail DESC;
```

## Exercice 3 :
```sql
SELECT * FROM eleves WHERE noms = 'Dupond';
SELECT * FROM eleves ORDER BY eleves ASC;
SELECT DISTINCT 

```