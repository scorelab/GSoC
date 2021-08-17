# Webiu

## Student Information

- Name - Yash Vardhan
- Email - yashvardhan513@gmail.com
- University - Indian Institute of Technology (Indian School of Mines) Dhanbad, India
- GitHub Profile - https://github.com/Grumpyyash
- Medium - https://yash-dn.medium.com/
- LinkedIn - https://www.linkedin.com/in/yash-vardhan-688952188/

# Project Abstract

![Dashboard](https://github.com/Grumpyyash/Webiu/raw/master/static/images/logo.png)

Webiu is a generalized website builder which eases the essential process of getting a website up and running easily. The project provide almost all of the different sections required by a normal website. This project focuses at implementing new features and functions into the current project to make it more reusable and accessible. Creating a logo, improving current components functionally, developing new Gatsby components, creating an NPM package for Webiu, visualizing the components using Storybook, refactoring one website built using webiu, deploying and publishing all sites are some key features of the project. This project functionally improves the current project, increase the range of the project and make the components accessible to other developers to incorporate them for developing websites.

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4834650184220672)

## [GSoC Project Proposal](https://docs.google.com/document/d/10a62w_QECCGDjTownzpFAUd_VFEzU1MZLmduVr4Duck/edit?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/Webiu)

## [GitHub Personal Repo](https://github.com/Grumpyyash/Webiu)

## [Commits during GSoC 2021](https://github.com/scorelab/Webiu/commits?author=Grumpyyash)

## [GSoC Blog](https://yash-dn.medium.com/)

# Work Summary

### Below is a comprehensive list of the milestone that were achieved during the coding period -

### 1) Functionality Improvement and Features Addition in Current Components

Improved and Refactor all the previously present components, fixed bugs, added new features and made the components more reusable. For e.g. Improve the GitterRoomList Component to fetch data related to all the rooms of an organization using Gitter APIs, Integrated the search functionality in projects list component etc.

Pull Requests for this milestone are -

- [Pull 1](https://github.com/scorelab/Webiu/pull/173)
- [Pull 2](https://github.com/scorelab/Webiu/pull/176)
- [Pull 3](https://github.com/scorelab/Webiu/pull/178)

### 2) Creation of Several New Reusable Gatsby Components

Created many reusable gatsby components, both static as well as dynamic based on API calls and other logic. The components are highly reusable and easily pluggable into any website. For e.g. created extensive components for GitHub APIs, Carousel, Timeline, Testimonial, Typewriter, and other general components etc.

Pull Requests for this milestone are -

- [Pull 4](https://github.com/scorelab/Webiu/pull/179)
- [Pull 5](https://github.com/scorelab/Webiu/pull/180)
- [Pull 6](https://github.com/scorelab/Webiu/pull/181)
- [Pull 7](https://github.com/scorelab/Webiu/pull/182)

### 3) Developing an NPM package for webiu

NPM package is a good way to increase the range of any project as it allows other to use our project. Generated the modules for all of the webiu components and pushed them into the package. Also, published the npm-package to npm-registry and made a project explaing the use-cases of the package.

Pull Requests for this milestone are -

- [Pull 8](https://github.com/scorelab/Webiu-npm/pull/1)
- [Pull 9](https://github.com/scorelab/Webiu-npm/pull/2)
- [Pull 10](https://github.com/scorelab/Webiu-npm/pull/3)

Also, the npm-package is published at - https://www.npmjs.com/package/webiu-npm

And, the sample project built explaining the use-cases - https://grumpyyash.github.io/webiu-npm-test/

### 4) Storybook Visualization of All Components

Storybook is a modern and a very powerful tool for dealing with components and wireframes. It gives a visual output of different components and makes it easy to see what is going on and how props are affecting a component. I added the storybook documentation for all the components as stories and published it live.

Pull Requests for this milestone are -

- [Pull 11](https://github.com/scorelab/Webiu/pull/184)

The storybook is deployed live at - https://grumpyyash.github.io/Webiu

And, on chromatic - https://610d0e8b03a01e003b2f5070-rllntdhgdq.chromatic.com/

### 5) Markdown Documentation and a Logo for Webiu

All the components are well-documented with one example usage per component, documented repository and its sub-parts with templates and guidelines for contribution. Also, created a logo for the project. Infact, created 4-5 logos out of which the best is chosen.

Pull Requests for this milestone are -

- [Pull 12](https://github.com/scorelab/Webiu/pull/170)
- [Pull 13](https://github.com/scorelab/Webiu/pull/172)
- [Pull 14](https://github.com/scorelab/Webiu/pull/183)
- [Pull 15](https://github.com/scorelab/Webiu/pull/164)

All the created logos can be found at - https://www.figma.com/file/LfhcLPkLKUOYOJsknKSxVy/Webiu-Proposed-Logo?node-id=3%3A2

### 6) Refactoring of the Leopards Lab website with correct data

The Leopards Lab website, built using the webiu components initially had all the dummy data in graphql queries. Extracted the correct data from GitHub and other resources and managed the queries to populate the site with correct data and deployed the website.

Pull Requests for this milestone are -

- [Pull 16](https://github.com/leopardslab/leopardslab.github.io/pull/1)
- [Pull 17](https://github.com/leopardslab/leopardslab.github.io/pull/2)

For the time being, the Leopards Lab website can be found at - https://grumpyyash.github.io/leopardslab.github.io/

# What's Covered

I was able to achieve almost all the milestones that we had discussed and I already discussed the major ones above. Overall, my work could be covered into -

- Refactored the current components functionally and added new features and fixed bugs
- Created a search bar and integrated it with projects, team and other components
- Implemented several GitHub components like- user, organization, repository etc. using GitHub APIs
- Created several new static reusable components like- Carousel, Timeline, Testimonial, FAQs, Cards etc.
- Created several new dynamic reusable components like - Timestamp, Countdown, Typewriter etc.
- Tweaked the current Gitter Room List component to show all the rooms of an organization instead of where the user is present
- Created a few logos for the project out of which one got selected as the official logo
- Created the base repository for npm-package and set up the base project
- Created modules for all the components, pushed it to the package and published to npm-registry
- Created a sample-project based on npm-package explaining the use-cases of the package
- Initialized storybook into the project and wrote stories for all of the webiu components
- Document all components, projects and sub-projects with storybook and markdown files and depoloyed the storybook
- Refactored the Leopards Lab website, populate it with the correct data and theme and deployed the site

My Task Tracker during whole of the GSoC coding period could be found at - https://indecisive-salesman-fde.notion.site/53fb00ab909142aca74a758a1dd9ca45?v=eb3c383e568046c8a5b260699a507e49

# What's left and future Aspects

Although I was able to complete almost all of the pre-decided milestones, a few features and ideas that would benefit the project and might implement in future are-

- Adding and writing tests for the components
- Creating 3-4 websites using webiu for different cases and differnet themes

# References

- [Gatsby Documentation](https://www.gatsbyjs.org/)
- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [NPM Registry](https://docs.npmjs.com/)
- [Storybook Documentation](https://storybook.js.org/docs/react/get-started/introduction)
- [Figma Docs](https://www.figma.com/)
- [GitHub Pages](https://docs.github.com/en/pages)
- [GitHub APIs](https://developer.github.com/v3/)
