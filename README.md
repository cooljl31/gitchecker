#GitChecker
GitChecker is an open source tool which aggregates statistics about Github projects. 

Have you ever been stuck wondering whether or not to use a library or a framework, uncertain of how well it was maintained? Help is here!

##Installation
```
$ git clone git@github.com:madshargreave/gitchecker.git
$ cd gitchecker

$ mix deps.get
$ npm install

```

##Running in development
Two run the application locally, the database must be prepared and an Github access token must be specified to be used in conjunction with the GitHub API.

###Database
Run the following commands to create and migrate the database

```
$ mix ecto.create
$ mix ecto.migrate
```


###Github Access Token
Before running locally, you must create an `.env` file in the project root.

Example `.env` file:


```
export GITHUB_ACCESS_TOKEN="your github access token"

```

###Starting servers
You must start both the webpack development server and the Phoenix server in seperate terminal tabs. For convenience, a `start` script has been suppliedin the project root to source the `.env` file before starting the webserver.

***Webpack (client):*** 
`npm start`

***Phoenix (server):*** 
`./start` or `source .env && mix phoenix.server`

##Stack

* Webpack
* Redux
* React
* React Router
* Elixir
* Phoenix
* PostgreSQL

##Contributing

Happy to accept any feedback, bug reports and pull requests

