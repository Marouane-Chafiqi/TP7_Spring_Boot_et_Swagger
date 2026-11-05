# TP 7 : Spring Boot et Swagger

Petite API REST pour gérer des étudiants, faite avec Spring Boot et MySQL, et documentée avec Swagger.

## Ce qu'il faut avant de lancer

- Java 17
- Maven
- MySQL 

## Lancer le projet

<img width="232" height="266" alt="image" src="https://github.com/user-attachments/assets/66f6cb83-c34a-41d5-89ca-7dbb8096ceee" />


```bash
mvn spring-boot:run
```

## Ce que fait l'API

Un étudiant a un `id`, un `nom`, un `prenom` et une `dateNaissance`.

| Méthode | URL | Ce que ça fait |
|---|---|---|
| POST | `/students/save` | Ajouter un étudiant |
| GET | `/students/all` | Voir tous les étudiants |
| GET | `/students/count` | Compter les étudiants |

Exemple pour ajouter un étudiant :

```json
{
  "nom": "Adnan",
  "prenom": "ENS",
  "dateNaissance": "2001-05-11"
}
```

## Swagger

Pas besoin de Postman : on teste tout depuis le navigateur sur
http://localhost:8080/swagger-ui/index.html



Quelques essais :

**Liste des étudiants**

<img width="1181" height="558" alt="Capture d&#39;écran 2026-11-05 194014" src="https://github.com/user-attachments/assets/0112935d-20e1-438e-b35d-d1dc71e6842f" />

**Ajout d'un étudiant**

<img width="1186" height="286" alt="Capture d&#39;écran 2026-11-05 194218" src="https://github.com/user-attachments/assets/48e82180-e317-4911-8d86-8bae8bfb163b" />

<img width="1086" height="552" alt="Capture d&#39;écran 2026-11-05 194311" src="https://github.com/user-attachments/assets/df0fa9da-2719-483f-bbda-1f2227ab91e0" />


