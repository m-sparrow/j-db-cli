# j-db-cli
j-db-cli is a client interface build on top of [j-db core engine] ()

## Syntax

```
Commands:
  jdb-cli.js create-db            Create Database
  jdb-cli.js list-all-dbs         Print list of Databases
  jdb-cli.js list-all-tables      Print list of tables
  jdb-cli.js scan-keys            Scan keys [primary, sort]
  jdb-cli.js create-table         Create a new table
  jdb-cli.js put-item             Add new item to the table
  jdb-cli.js get-item             Retrieve item from table
  jdb-cli.js update-item          Update an existing item in table
  jdb-cli.js delete-item          Delete an item from table
  jdb-cli.js add-item-element     Add an element to an Item
  jdb-cli.js remove-item-element  Remove an element from an Item

Options:
  --version      Show version number                                   [boolean]
  -c, --cmd      A valid db operation. Refer commands section         [required]
  -d, --db       Database
  -t, --table    Table Name
  -o, --options  [schema, keys, item, tags or/and values, etc]
  -h, --help     Show help                                             [boolean]

Examples:
  jdb-cli.js create-db -d [db-name]
  jdb-cli.js list-all-dbs
  jdb-cli.js list-all-tables -d [db-name]
  jdb-cli.js scan-keys -d [db-name] -t [table-name] -o [keys]
  jdb-cli.js create-table -d [db-name] -t [table-name] -o [schema]
  jdb-cli.js put-item -d [db-name] -t [table-name] -o [options]
  jdb-cli.js get-item -d [db-name] -t [table-name] -o [options]
  jdb-cli.js update-item -d [db-name] -t [table-name] -o [options]
  jdb-cli.js delete-item -d [db-name] -t [table-name] -o [options]
  jdb-cli.js add-item-element -d [db-name] -t [table-name] -o [options]
  jdb-cli.js remove-item-element -d [db-name] -t [table-name] -o [options]
```
