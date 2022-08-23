# search-service-es-ubx2-api

`DESCRITPION:` A search service to build up ElasticSearch queries and interact with ES to fetch the search results.

Basic Tools Required to run the application:`NodeJS`  `typescript` 

Master Branch: master


## Contents

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents :arrow_down: </summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
         <li><a href="#contents">Project Repo</a></li>
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
        <li><a href="#start-app">Start App</a></li>
        <li><a href="#travis-build-link">Travis Build Link</a></li>
        <li><a href="#sonar-coverage">Sonar Coverage</a></li>
        <li><a href="#run-tests">Run Tests</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#deployment">Deployment</a></li>
  </ol>
</details>

## Built With


**Programming Languages**

<img title="Typescript" alt="Typescript" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/typescript/typescript.png" />|<img alt="JS" title="JavaScript" width="40px" src="https://raw.githubusercontent.com/github/explore/master/topics/javascript/javascript.png">
|--|--|



**Libraries and Frameworks**
<img title="express" alt="express" width="40px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/express/express.png">|<img title="node" alt="node" width="40px" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg">
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

## Getting started

### Required tools

Required tools to setup and build service.
-NodeJs:
  - [Nodejs](https://nodejs.org/en/docs/): Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
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
# search-service-es-ubx2-api
git clone  https://github.com/tandfgroup/search-service-es-ubx2-api

# change directory to repo
cd search-client-ubx2-website

```
### Install application and dependencies

```bash
npm login --registry https://npm.taylorfrancis.com
#enter the username, password, email
```

```bash
npm install --registry https://npm.taylorfrancis.com
```


### Build app


```bash
npm run build
```
### Start app

```bash
npm run start

# To start the `nodemon` so that which every change you make in repository, it watches for changes and builds and starts the application again. 
# npm run dev
```

### Run tests
```bash
npm run test
```

### Travis Build Link


`Travis Build Link:` https://travis-ci.com/github/tandfgroup/search-service-es-ubx2-api?utm_campaign=ww_en_brand&utm_medium=cpc&utm_source=google&utm_term=travis%20ci

### Sonar Coverage

`Sonar Coverage:` https://sonarcloud.io/dashboard?id=tandfgroup_search-service-es-ubx2-api

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
`--Thank you --😊`
