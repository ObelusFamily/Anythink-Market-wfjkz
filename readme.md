# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

### Pre-requisites

- Docker - Please install the latest version of docker for your platform. Instructions can be found on the [docker website](https://docs.docker.com/get-docker/)
- Docker compose - This should typically be installed alongwith your docker install, but if not, please also install `docker-compose`

### First-run setup

The local environment has been setup as a docker-compose application. In order to run the application locally, run the following command in the root directory of the project:

```shell
docker compose up # (or docker-compose up, if using an older version of docker with docker-compose installed as a separate binary)
```
- Verify that the backend is running by navigating to http://localhost:3000/api/ping
  - You should see a JSON response: `Pong! Seems like Everythink is working, great job!"
- Verify that the frontend is running by naviagating to http://localhost:3001/register
- Create a new account, this will be your local testing account

Read through the `docker-compose.yml` file in the root directoy to understand the local setup better.
