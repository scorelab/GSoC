# Node Cloud: Implement development road-map

## Student Info

* Name - Rajitha Warusavitarana
* Email - rajitha.2017310@iit.ac.lk, rajitha1998@gmail.com
* University - Informatics Institute of Technology
* GitHub Profile - https://github.com/rajitha1998
* LinkedIn profile - https://www.linkedin.com/in/rajithawaru/
* Medium - https://medium.com/@rajitha1998
* Twitter - [rajebro](https://twitter.com/rajebro)

### Project Abstract

**`NodeCloud ☁️`** is standard library to get a single API on the open cloud with multiple providers. It is a NodeJs library which comes with plugins for each cloud provider. NodeCloud's aim is to abstract away the differences between different cloud providers. It provides an easy to use API for developers in order to interact with different cloud providers.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4606652017278976)

### [GSoC Project Proposal](https://docs.google.com/document/d/1J0K6E3MmMjg55Lu0_cvmuHa8_t_mfSRG/edit#)

### [GitHub Organization Repo](https://github.com/leopardslab/nodecloud)

### [GitHub Personal Repo](https://github.com/rajitha1998/nodecloud)

### Commits during GSoC 2020

 * [PR 1](https://github.com/leopardslab/nodecloud-aws-plugin/pull/29)
 * [PR 2](https://github.com/leopardslab/nodecloud-aws-plugin/pull/30)
 * [PR 3](https://github.com/leopardslab/nodecloud-gcp-plugin/pull/32)
 * [PR 4](https://github.com/leopardslab/nodecloud/pull/47)
 * [PR 5](https://github.com/leopardslab/nodecloud/pull/46)
 * [PR 6](https://github.com/leopardslab/nodecloud/pull/48)
 * [PR 7](https://github.com/leopardslab/nodecloud/pull/49)
 * [PR 8](https://github.com/leopardslab/nodecloud/pull/51)
 * [PR 9](https://github.com/leopardslab/nodecloud/pull/55)
 * [PR 10](https://github.com/leopardslab/nodecloud/pull/58)
 * [PR 11](https://github.com/leopardslab/nodecloud/pull/59)
 * [PR 12](https://github.com/leopardslab/nodecloud/pull/62)
 * [PR 13](https://github.com/leopardslab/nodecloud/pull/63)

### Project Demo Video

 * YouTube: https://youtu.be/UaPd-kZBDWE
 * Google drive: https://drive.google.com/file/d/1P8VhPb2fnaNAl79vsH4Omh9SLybkqALi/view?usp=sharing

### GSoC Blog

 * [GSoC 2020: Beginning of a New Adventure](https://medium.com/leopards-lab/gsoc-2020-beginning-of-a-new-adventure-33ae2ae3df13)
 * [GSoC 2020: Getting familiar with the playground](https://medium.com/leopards-lab/gsoc-2020-getting-familiar-with-the-playground-5f5d736a9157)
 * [GSoC 2020: One more week left in the community bonding period](https://medium.com/leopards-lab/gsoc-2020-one-more-week-left-in-the-community-bonding-period-f13b77b44a8f)
 * [GSoC 2020: Coding is Official!](https://medium.com/leopards-lab/gsoc-2020-coding-is-official-b3b379128098)
 * [GSoC 2020: Parsing, Transforming and Generating](https://medium.com/@rajitha1998/gsoc-2020-parsing-transforming-and-generating-613e27d7459b)
 * [GSoC 2020: Finally! Automated code generation for Node Cloud Azure plugin](https://medium.com/leopards-lab/gsoc-2020-finally-automated-code-generation-for-node-cloud-azure-plugin-62e645cd9add)
 * [GSoC 2020: Diving into Google Cloud SDKs](https://medium.com/@rajitha1998/gsoc-2020-diving-into-google-cloud-sdks-e3c6192a077e)
 * [GSoC 2020: Easy package management with Lerna](https://medium.com/leopards-lab/gsoc-2020-easy-package-management-with-lerna-65c2ca0c2237)
 * [GSoC 2020 : Automated code generation using Google cloud Client based SDKs](https://medium.com/@rajitha1998/gsoc-2020-automated-code-generation-using-google-cloud-client-based-sdks-e7dedb936a79)
 * [GSoC 2020: Completing the Transformers for Google Cloud plugin](https://medium.com/@rajitha1998/gsoc-2020-completing-the-transformers-for-google-cloud-plugin-2d48da3df7c8)
 * [GSoC 2020: Tasty Testing with Mocha and Chai ☕️](https://medium.com/leopards-lab/gsoc-2020-tasty-testing-with-mocha-and-chai-%EF%B8%8F-6f7452a2e4eb)
 * [GSoC 2020: Documentation is equally important as code 📚](https://medium.com/@rajitha1998/gsoc-2020-documentation-is-equally-important-as-code-f78a79440b0f)
 * [GSoC 2020: Working on the Final Touches 🖌️](https://medium.com/@rajitha1998/gsoc-2020-working-on-the-final-touches-%EF%B8%8F-7f0a71f152c6)

### Work Summary

 NodeCloud is an open-source project under SCoRe Lab. Initially, I was aimed to enhance Node cloud by manually implementing new services in AWS, Google Cloud and Azure plugins. But after an awesome suggestion of my mentor Rajika Imal it was decided to automatically generate the NodeCloud plugins classes through code generation. so as to achieve it TypeScript’s compiler API was used to parse SDK files to extract required data, and well as to transform source code to generate the Node Cloud plugin classes. The required parsers, transformers and other functionalities for this automated process is developed for the AWS, GCP and Azure plugins. Furthermore, the core module and the AWS, GCP and Azure plugins are now located in the same repository(mono repo) managed with Lerna. The API documentation of these plugins is automatically generated with the help of JSDoc and TypeScript’s compiler API.

### What Covered

 * Implemented parsers, transformers and generators in the code generation component for AWS, GCP and Azure. 
 * Structuring the project as a monorepo with Yarn and Lerna.
 * Created dummy data for unit testing and Wrote unit tests for the code generation component.
 * Automating the API documentation process with JSDoc and Typescript compiler API.
 * Updating the documentation of the NodeCloud project.
 * Finalizing the `node-cloud.yml` file.
 * Generating the JavaScript classes for NodeCloud plugins and updating the plugins with them.

 **Github Issues**

 * [Issue 1](https://github.com/leopardslab/nodecloud/issues/52)
 * [Issue 2](https://github.com/leopardslab/nodecloud/issues/50)
 * [Issue 3](https://github.com/leopardslab/nodecloud/issues/54)
 * [Issue 4](https://github.com/leopardslab/nodecloud/issues/57)
 * [Issue 5](https://github.com/leopardslab/nodecloud/issues/56)
 * [Issue 6](https://github.com/leopardslab/nodecloud/issues/61)
 * [Issue 7](https://github.com/leopardslab/nodecloud/issues/60)
 * [Issue 8](https://github.com/leopardslab/nodecloud/issues/31)

### What left

 * More cloud services can be generated by updating the `node-cloud.yml` file. 

### Reference

 * [Writing typescript custom AST transformer part-1](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-1-7585d6916819)
 * [Writing typescript custom AST transformer part-2](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-2-5322c2b1660e)
 * [Writing typescript custom AST transformer part-3](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-3-93b6238ae21f)
 * [Guide for lerna with yarn-workspaces](https://medium.com/@jsilvax/a-workflow-guide-for-lerna-with-yarn-workspaces-60f97481149d)
 * [TypeScript unit testing](https://medium.com/swlh/typescript-unit-testing-with-test-coverage-2cc0cc6f3fd1)
 * [Lerna Crash Course](https://www.youtube.com/watch?v=p6qoJ4apCjA&list=LLh83suuTLe5XvJS2qjzem8Q&index=93&t=0s)
 * [JSDoc Crash Course](https://www.youtube.com/watch?v=YK-GurROGIg&list=LLh83suuTLe5XvJS2qjzem8Q&index=19&t=0s)
