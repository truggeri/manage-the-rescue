# Manage the Rescue

Manage the Rescue (MtR) is a free to use web application attempting to aid animal rescue organizations with animal tracking services.

This project is in active development. It is written using Ruby on Rails, VueJS and Tailwind CSS.

## Environment Setup

The following describes how to setup a development environment.

### Ruby and Rails

This project uses Ruby 2.6.2 and Rails 6.0.0.

### Environment Variables

The following variables are used by the application. I would recommend putting something like the following in a .env file.

```bash
export MANAGE_THE_RESCUE_DB_DATABASE=dev-database
export MANAGE_THE_RESCUE_DB_USERNAME=dev-user
export MANAGE_THE_RESCUE_DB_PASSWORD=
export DATABASE_URL=postgres://$MANAGE_THE_RESCUE_DB_USERNAME:$MANAGE_THE_RESCUE_DB_PASSWORD@localhost:5432/$MANAGE_THE_RESCUE_DB_DATABASE
```

### Database

This project uses Postgres as a persistent data store. In order to setup a database from within a Docker container, run the following command.

```bash
docker run --name mtr-db -p 5432:5432 -e POSTGRES_PASSWORD=$MANAGE_THE_RESCUE_DB_PASSWORD -e POSTGRES_USER=$MANAGE_THE_RESCUE_DB_USERNAME -e POSTGRES_DB=$MANAGE_THE_RESCUE_DB_DATABASE -v /Users/truggeri/code/manage-the-rescue/data/pg:/var/lib/postgresql/data -d postgres:11.1
```
