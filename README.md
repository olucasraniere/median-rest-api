## Median - A simples blog REST API

A simple backend REST API for a blog built using NestJS, Prisma, PostgreSQL and Swagger.
The project was developed following the instructions in the article 'Building a REST API with NestJS and Prisma' available at:

- https://www.prisma.io/blog/nestjs-prisma-rest-api-7D056s1BmOL0
- https://www.prisma.io/blog/nestjs-prisma-validation-7D056s1kOla1
- https://www.prisma.io/blog/nestjs-prisma-error-handling-7D056s1kOop2
- https://www.prisma.io/blog/nestjs-prisma-relational-data-7D056s1kOabc
- https://www.prisma.io/blog/nestjs-prisma-authentication-7D056s1s0k3l

### Installation

1. Install dependencies: `npm install`
2. Rename the `.env.example` file to `.env` and change the database access data according to your scenario
3. Start a PostgreSQL database with docker using: `docker compose up -d`.
   - If you have a local instance of PostgreSQL running, you can skip this step. In this case, you will need to change the `DATABASE_URL` inside the `.env` file with a valid [PostgreSQL connection string](https://www.prisma.io/docs/concepts/database-connectors/postgresql#connection-details) for your database.
4. Apply database migrations: `npx prisma migrate dev`
5. Start the project: `npm run start:dev`
6. Access the project at http://localhost:3000/api
