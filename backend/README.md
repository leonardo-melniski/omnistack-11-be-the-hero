## knex 

### Config

```
module.exports = {

  development: {
    client: 'sqlite3',
    connection: {
      filename: './src/database/db.sqlite'
    },
    migrations: {
      directory: './src/database/migrations'
    },
    useNullAsDefault: true
  }

}
```

### Usage of migration

create

`$ npx knex migrate:make <migration_name>`


execute

`$ npx knex migrate:latest`