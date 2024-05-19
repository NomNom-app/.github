# NomNom
Android app for sharing restaurant reviews with friends.

## About the project
NomNom app is a social platform for sharing restaurant reviews, built using React Native for the frontend and ASP.NET for the backend. Users can log in, place pins on a map to mark the location of a restaurant they've visited, and leave a review in a post associated with the pin. This post includes the restaurant's name, the date of the visit, and the review itself. Friends can then view these pins and leave comments on the posts.

The backend of the application is an ASP.NET Web API that communicates with a PostgreSQL database. The database is hosted on Google Cloud Compute Engine, and the API is deployed on Google Cloud Run. The API uses Entity Framework, a popular ORM, to query the PostgreSQL database. This allows the application to work with the database using .NET objects, simplifying data access.

The application's development process is automated using GitHub Actions. When changes are pushed to the development branch of the backend repository, GitHub Actions builds a new Docker image and pushes it to Google Artifact Registry. This image is then deployed to a service on Google Cloud Run.

This setup allows for a streamlined development process, as changes can be easily tested and deployed. It also ensures that the application can scale to handle increased load, as Google Cloud Run can automatically adjust the number of service instances based on incoming traffic.

## Architecture
![arch](https://github.com/NomNom-app/.github/assets/61557728/01ca4145-48f7-47db-9fe9-47a4a69a8410)

## Testing reports
- [Testing plan](../docs/testPlan.pdf)
- [Unit tests](../docs/unitTests.pdf)

## Documentation
- [User manual](../docs/userManual.pdf)

## Authors
Evita Šriupšaitė  
Lukas Andrijauskas  
Rugilė Petraitytė  
Ieva Žukauskaitė
