# Project Name

CLocal-Azure

## Student Info

* Name - Lakindu Gunasekara
* Email - lakindu1995@gmail.com
* University - Informatics Institute of Technology, Sri Lanka
* GitHub profile - https://github.com/lakindu95
* LinkedIn profile - https://www.linkedin.com/in/lakindu-gunasekara

### Project Abstract

CLocal Azure is an local emulator to test or mock the Azure Services without deploying into Azure Platform, and provide easiness for developer by reducing the cost. Our goal is to have all azure possible local services into one single project and provide easiness to run a whole azure project locally. Currently the project supports up to 8 services and 4 of them were written during the GSoC 2019 period.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5495000714969088)

### [GSoC Project Proposal](https://drive.google.com/file/d/1qoZ0FixFzzqqG0AczDo1sxSultLNMqls/view?usp=sharing)

### [GitHub Organization Repo](https://github.com/cloudlibz/clocal-azure)

### [GitHub Personal Repo](https://github.com/lakindu95/clocal-azure)

### Commits during GSoC 2019

* [Pull Request 1](https://github.com/cloudlibz/clocal-azure/pull/56)
* [Pull Request 2](https://github.com/cloudlibz/clocal-azure/pull/57)
* [Pull Request 3](https://github.com/cloudlibz/clocal-azure/pull/58)

### [Project Demo Video](https://www.youtube.com/playlist?list=PLbd4A5tkijhDGRQp6BcrwGhRvS0TU8zhQ)

### [Project Wiki](https://github.com/cloudlibz/clocal-azure/wiki)

### [GSoC Blog](https://medium.com/tag/clocal-azure/latest)

### Work Summary

During the period of 2019, I have been adding more services to CLocal Azure project. The added services are mentioned below and one of the services are written from scratch covering the basic functioanlities.

Services added,
- Azure CLI
- Azure SQL Server
- Azure KeyVault
- Azure Search (Built from scratch)

To add value to the services above, a video demo series has been added to the clocal azure youtube playlist and weekly medium articles were written to give the updates of the progress. For more information regarding the summary please see the link below.

* [GSoC Summary](https://medium.com/@lakindu1995/gsoc-2019-summary-fbafcb351cdc)


### What Covered

For the GSoC period, I have covered the following services. 

1. Azure CLI (cli start, cli stop)
2. Azure SQL Server (sql start, sql stop)
3. Azure KeyVault (vault start, vault stop)
4. Azure Search (search start, search stop)

- To run all services at once, added a shell script (sh compose.sh)

### What left

- Add more services to emulate.
- Add more features on Azure Search service.

### Reference

- [Quickstart: Create an Azure Search index in Node.js](https://docs.microsoft.com/en-us/azure/search/search-get-started-nodejs)
- [Search Documents (Azure Search Service REST API)](https://docs.microsoft.com/en-us/rest/api/searchservice/Search-Documents)
- [CREATE INDEX (Transact-SQL)](https://docs.microsoft.com/en-us/sql/t-sql/statements/create-index-transact-sql?view=sql-server-2017)
- [How to run HashiCorp Vault (Secrets Management) in Docker](https://www.melvinvivas.com/secrets-management-using-docker-hashicorp-vault/)
