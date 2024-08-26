# CMPG-323-Overview-30512948

PROJECT 1

This repository has been created for the use of project one for the linked Kanban planning project showing the implementation of Scrum in Agile framework and source controlling. This repository will also store the documentation for project one and a burndown chart.

In projects two to five, a branching strategy of creating a feature branch from the main branch where changes will be committed and pull requests will be submitted before merging the feature branch into the main branch and deleting the feature branch.

In project two, the .gitignore will be used to ignore .NET files and directories each time a commit is made.

In project two, security for the storage of credentials and sensitive information will be used for the web API.

PROJECT 2

This project is a web application programming interface (API) project that a client of NWU Tech Trends will use to interact with a connected database in an application, storing telemetry data, using web services over HTTP commands/ verbs. This API is a RESTful API as the webpage adheres to the representational state transfer (REST) model and architectural style.

The user may use CRUD methods (create, read, update, delete) to manipulate data stored on the database. The client then initiates a request to a server endpoint by use of the HTTP commands/ verbs GET, POST, PUT, DELETE. These commands/ verbs are explained below:

POST — sends data that creates a resource (C: create)
GET — fetches a resource and returns the data (R: read)
PUT — sends data that updates a resource (U: update)
DELETE — removes a resource (D: delete)

Endpoints may be with or without parameters. Those without parameters allow for data manipulation for the entire database resource table. Those with parameters, a unique identifier, only allow for data manipulation with a specific resource.

The endpoints for data manipulation in the database are:

GET/api/Clients
GET/api/Clients/{id}
POST/api/Clients
PUT/api/Clients/{id}
DELETE/api/Clients/{id}

GET/api/Processes
GET/api/Processes/{id}
POST/api/Processes
PUT/api/Processes/{id}
DELETE/api/Processes/{id}

GET/api/Projects
GET/api/Projects/{id}
POST/api/Projects
PUT/api/Projects/{id}
DELETE/api/Projects/{id}

GET/api/JobTelemetries
GET/api/JobTelemetries/{id}
POST/api/JobTelemetries
PUT/api/JobTelemetries/{id}
DELETE/api/JobTelemetries/{id}

PROJECT 3

NWU Tech Trends Web App.

This project is an ASP.NET Core Web App that uses Model, View, and Control (MVC) with Entity Framework Core to manage the Project and Client entities. A repository pattern is used to separate data access operations from the controller class to improve maintainability and testability.

A repository pattern is used to separate data access logic from the ProjectsController and ClientController classes by moving it into a ProjectRepository and ClientRepository respectively. This change makes the controller classes more focused on handling HTTP requests and responses, and the repository classes managing all database operations; it interacts directly with the TechtrendsContext to perform CRUD operations. The ProjectsController and ClientsController classes will then use the ProjectRepository and ClientRepository classes respectively to handle data operations.

The benefits of using a repository pattern is that it removes the need to recreate controller methods every time logic changes. By moving data access logic to the repository, it makes the controller class cleaner and more focused on request handling, as they are entrypoints into the application. Centralising data access logic in the repository simplifies changes and testing of data operations. Reusability is also promoted as repository methods can be reused across different parts of the application, reducing code redundancy.
