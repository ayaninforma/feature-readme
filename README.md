# search-client-ubx2-website

This Web application serves the search page across multiple projects.


<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->


## Contents

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents :arrow_down: </summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
         <li><a href="#contents">Project Repo</a></li>
         <li><a href="#libs">Libs</a></li>
      </ul>
    </li>
    <li>
      <a href="#built-with">Built with</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#required-tools">Required tools</a></li>
        <li><a href="#system-dependency">System dependency</a></li>
      </ul>
    </li>
     <li>
      <a href="#clone-repository">Clone repository</a>
    </li>
      <li>
      <a href="#install-application-and-dependencies">Install application and dependencies</a>
      <ul>
        <li><a href="#build-app">Build App</a></li>
        <li><a href="#run-tests">Run Tests</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#deployment">Deployment</a></li>
  </ol>
</details>

## Built With


**Programming Languages**

<img title="Typescript" alt="Typescript" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/typescript/typescript.png" />|<img alt="JS" title="JavaScript" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/javascript/javascript.png">|<img title="Java" alt="java" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/java/java.png">
|--|--|--|



**Libraries and Frameworks**

<img title="Angular" alt="Angular" width="40px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/angular/angular.png">|<img title="express" alt="express" width="40px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/express/express.png">
|--|--|


**Cloud**

<img title="AWS" alt="AWS" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/aws/aws.png">|
|--|

**Databases**

<img title="SQL" alt="SQL" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/sql/sql.png">|<img title="MongoDB" alt="MongoDB" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/mongodb/mongodb.png">|<img title="ElasticSearch" alt="ElasticSearch" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/elasticsearch/elasticsearch.png"> <br>
|--|--|--|

**Tools**
<img title="VS Code" alt="VS Code" width="40px" src="https://img.icons8.com/fluent/48/000000/visual-studio-code-2019.png">|<img title="git" alt="git" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/git/git.png">
|--|--|
<br>



### Libs

[cloudflare-lib](https://github.com/tandfgroup/discovery-client-websites/tree/develop/libs/cloudflare-lib) - Utility code and cloudflare workers[WIP for webpack].

[prerender-lib](https://github.com/tandfgroup/discovery-client-websites/tree/develop/libs/prerender-lib) - Utility code for all the pre rendering lambdas.

[shared-lib](https://github.com/tandfgroup/discovery-client-websites/tree/develop/libs/shared-lib) - All shared components, services and utils


## Getting started

### Required tools

Required tools to setup and build service.

- [Angular](https://angular.io/): Angular is an app-design framework and development platform for creating efficient and sophisticated single-page apps.
- TypeScript:
  - [TypeScript](http://www.typescriptlang.org/): A superset of JavaScript that compiles to clean JavaScript output.
  - [@types](https://www.npmjs.com/~types): TypeScript definitions for Node modules.
  - [ESLint](https://eslint.org/): ESLint checks your TypeScript code for readability, maintainability, and functionality errors.
- Unit Testing:
  - [Karma](https://angular.io/guide/testing): This guide offers tips and techniques for unit and integration testing Angular applications.


### System dependency


Your system will need access to [`node`](https://nodejs.org/en/) v9+ and [`npm`](https://www.npmjs.com/) v3+.

With Node/npm installed, you should install these globals with `npm install --global`:

## Clone repository

```sh
# --depth 1 removes all but one .git commit history
git clone  https://github.com/tandfgroup/search-client-ubx2-website.git
search-client-ubx2-website

# change directory to repo
cd search-client-ubx2-website

```
### Install application and dependencies <a id="install-app"></a>

```bash
npm login --registry https://npm.taylorfrancis.com
```

```bash
npm install --registry https://npm.taylorfrancis.com
```


### Build app


```bash
npm run prerender:dev
```

### Run tests

```bash
npm run test
```

## Contributing

Please fork the repo and create a pull request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## Deployment


There are readme files in each app which describes how to setup each project and do the local development. Deployments are done using Github Actions. All the apps are deployed using specific tags that are defined in the [build script](https://github.com/tandfgroup/discovery-client-websites/blob/develop/.github/workflows/deploy.yml).

Create a release from the Github website with proper release notes. This helps in auditing as well. Choose the correct branch to deploy from and also create the correct tag. The application will be deployed based on the tag.

The tag follows a particular pattern like `<app>/*/[1-9]+.[0-9]+.[0-9]+`.
for example, to deploy product pages to uat green, the tag would be `product/u-g/2.0.3` and so on.

There is a lot of scope for improvements in the deploy scripts and tagging patterns. PRs are welcome


```bash
 serverless deploy --stage ${ENVIRONMENT}
```



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
