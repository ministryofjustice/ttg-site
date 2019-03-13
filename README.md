# Through the Gate - POC

## Dev Enviroment Setup

- NVM - [Node Version Manager](https://github.com/creationix/nvm): `nvm use`
- Docker

## Running app via Docker

### Config

- `/server/confg.js` for properties availible to configure all with sensible defaults
- Create a .env to customise these values or override

### Docker

- pull latest container: `docker-compose pull`

- run container stack: `docker-compose up -d`

- run docker setup scripts (managed by knex.js): docker exec {{ttg container}} npm run migrate

- monitor log output: `docker logs -f {{ttg container id}`

- navigate to http://localhost:3000

## Notes

- Cloned from [Form app starter](https://github.com/ministryofjustice/form-app-starter/commit/1e88ef7f96fb48431006b350700200f12d71ef65)
