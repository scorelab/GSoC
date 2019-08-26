# OpenMF - Redesign Androphsy(OpenMF) backend in Python

## Student Info
- Name - Harish Ghunawat
- Email - harish.ghunawat1@gmail.com
- University - IIT Roorkee
- Github Profile - [Wolf-Legend](https://github.com/wolf-legend)
### Project Abstract
OpenMF is an Android forensic tool, developed in Python. OpenMF consists following features
- Common Databases extraction
- Data conversion tools (ex. db to csv)
- Session records (handling multiple cases/projects)
- Generating report of projects
- Created light-weigth CLI for easily using these features

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5283093169045504)

### [GSoC Project Proposal](https://docs.google.com/document/d/1KboOKdS9sBDcb8hceNKlclwB_QnAaOPFGVQHUC9cyg4/edit)

### [GitHub Organization Repo](https://github.com/scorelab)

### [GitHub Personal Repo](https://github.com/scorelab/OpenMF)

### [Commits during GSoC 2019](https://github.com/scorelab/OpenMF/commits?author=Wolf-Legend)

### [Project Demo Video](https://drive.google.com/open?id=1QALmBtviYctsFUktlHkdp_zHkuT48aFd)

### [Project Wiki](https://github.com/scorelab/OpenMF/wiki)

### Work Summary
- Made project Cross-platform compatible
- Make a basic python backend to access and acquire data
from android and providing super-user access to user i.e.
rooting the android device if it’s not already rooted
- Added multi-user and multi-case support for the this basic
backend
- Report generation in generic html, txt and PDF reports formats at
the end
- Added support for sqlite for the database management of both user,case
and for extraction and analysis of databases acquired from
android
- Created light-weight CLI for using these features 
- Written module for generation of basic report in neat
templates
- Tested the fully working python backend based
Androphsy(OpenMF)
### What Covered
1. Basic Android forensic tool ready for use
2. Added multiple features required for handling data extraction and manipulation
3. Create module for report generation for particular case
4. Developed light-weight CLI for supporting these features in just one command

### What left
1. Implementing Web-view of this project (WIP)
2. Writing down blogs about how to use this project effectively
3. Adding support for database analysis algorithms

### Reference
1. “scorelab/ANDROPHSY”-https://github.com/scorelab/androphsy
2. Python
3. [pdfkit](https://github.com/JazzCore/python-pdfkit)
4. SQLite
5. ADB
