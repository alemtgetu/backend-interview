## KUNGFUAI Forked

Using the NodeJS application framework NestJS, create a TODO list application that persists the TODOs to a database.

Features:

- Create a TODO
- Edit an existing TODO
- Delete an existing TODO
- See all of the todos

### Server Address

- http://100.25.157.4:3000

### Endpoints

- /tasks, Get -- list all tasks
- /tasks/:id, Get -- get on task
- /tasks, Post -- create/add a task
- /tasks/:id, Patch -- update/edit a task
- /tasks/:id, Delete -- delete/remove a task

Use any of the Cloud Providers listed below to deploy your solution

- AWS
- GCP
- Azure

### Deployed On AWS EC2

- API and dockerized Posgres DB are hosted on same EC2
- SG for the EC2 instance Inbound Rules looks as follows
  - Port 5432 open for only the instance's SG
  - Port 22 to allow connection coming only from my home IP
  - Port 3000 open to world (It's not good idea to open your applications port to world, reverse proxy will be much secure)
  - Port 80 open to the world (was planning to implement NestJs to listen on port 80 instead of 3000)

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).
