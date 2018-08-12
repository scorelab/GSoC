# Project Name

CLocal-Azure

## Student Info

* Name - Lakindu Gunasekara
* Email - lakindu1995@gmail.com
* University - Informatics Institute of Technology, Sri Lanka
* GitHub profile - https://github.com/lakindu95
* LinkedIn profile - https://www.linkedin.com/in/lakindu-gunasekara

### Project Abstract

CLocal Azure is an local emulator to test or mock the Azure Services without deploying into Azure Platform, and provide easiness for developer by reducing the cost. Our goal is to have all azure possible local services into one single project and provide easiness to run a whole azure project locally. Currently project supports azure functions, azure storage and azure cosmos db emulators to run locally. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5610489845907456)

### [GSoC Project Proposal](https://drive.google.com/open?id=1-VnJFRaNZNawGCZp38K6JRzd1C-6zoRP)

### [GitHub Organization Repo](https://github.com/cloudlibz/clocal-azure)

### [GitHub Personal Repo](http://github.com/lakindu95/clocal-azure)

### [Commits during GSoC 2018](https://github.com/cloudlibz/clocal-azure/pull/2)

### [Project Demo Video](https://www.youtube.com/playlist?list=PLbd4A5tkijhDGRQp6BcrwGhRvS0TU8zhQ)

### [Project Wiki](https://github.com/cloudlibz/clocal-azure/wiki)

### [GSoC Blog](https://medium.com/tag/clocal-azure/latest)

### Work Summary

For the GSoC 2018, I've initiate the project from the scratch and added support for four services to emulate locally. 

Services added,
- Azure Functions
- Azure Storage (Blob, Queue & Tables)
- Azure CosmosDB 
- API App Service

Along with the above implementations, I have added sample projects for each service in the project itself and added an article every week and created a video series for each service.

### What Covered

For the initial stage I have covered the following services. 

1. Azure Functions (function init, function start, function stop)
2. Azure Storage (storage start, storage clear, storage stop)
    - Blob
    - Queue
    - Table
3. Azure Cosmos DB (cosmosdb init, cosmosdb start, cosmosdb stop)
4. API App Service (api start)

- Added a script to run all services at once (sh compose.sh)

### What left

- Portential to add more services 
- Add additional commands for services 

### Reference

- [Azure Functions Documentation for Local Run](https://docs.microsoft.com/en-us/azure/azure-functions/functions-run-local)
- [Azure Cosmos DB Emulator](https://docs.microsoft.com/en-us/azure/cosmos-db/local-emulator)
- [Azure Storage Emulator](https://docs.microsoft.com/en-us/azure/storage/common/storage-use-emulator)
- [Azure API App Service sample](https://github.com/Huachao/azure-content/blob/master/articles/app-service-api/app-service-api-nodejs-api-app.md)