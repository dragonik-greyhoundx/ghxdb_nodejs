# GHXDB - NodeJs
## A three dimentional locator id database

A database concept based on a x;y;z id data to make a different logic of storage and make three dimentional data visualization.

[!WARNING]
This project just started and actually working on, based on a personal project to make locals databases easier to setup on small and personnal projects. If you are interested by the project, feel free to contact me on discord ( .dragonik ) or by mail ( guillaume.douchement@gmail.com )

## Concept of GHXDB
### Data "locator"
The data locator is similar to an id but have properties

| index | Description |
| x | Similar to tables in SQL, it's the main property of the data OR the main property while searching specified datas |
| y | It's a sub-main property or a required property of the data OR the second property while searching specified datas |
| z | It's the "id" of the data |

exemple of a locator => { x: 1, y: 1, z: 1 }

An index start at 1 for data entities but, while searching datas by specified properties, x must not be equal to zero but can be negative, y can be equal to zero ( 0 mean no target property ) and z can be 0 ( 0 mean no target data entity )

The locator { x: 0, y: 0, z: 0 } is the database admin locator

A data entity with a y equal to zero and/or z equal to zero is a config / property data entity

### The locator mutation
To perform search or database refactoring, GHXDB gonna make a process to modify x, y and z by desire properties. While searching on large amount of datas, the database gonna be able to store a replication of the origin and one with the mutation for better performance.

### Negative index
A negative index mean that the target data entity is archived or the lifecycle of the data entity is finish



### Working on :
* Database file management
* Database import and export process
* Defining and testing low and high security system (specify data and database access)