# todoAPI
grapghQL, API Flask, Ariadne

Learning about GraphQL used it to create a todo api app that allows to update due date, create new task, delete task

### GraphQL
GraphQL is a query language for APIs and a server-side runtime that allows clients to request only the data that is required. It uses the Schema Definition Language (SDL) which is used to write GraphQL schemas.

### Fetching Data
GraphQL provides a single endpoint from where client can request all the data that it needs by posting a query like this
          ```type Query {
              student_info: [Students]!
              }
           ```
           
### Creating and Modifying data
GraphQL provides a simple logic to create, update and delete data. it is called **mutation**. A mutation to create a new student information looks something like this
            ```type Mutation {
                  createStudentInfo(name: String!, age: Int!, gender: String!): Students!
                  }
                ```
The mutation accepts 2 strings and 1 integer and returns a Student object.

The first step in creating a graphQL API is designing the schema. i called mine schema.graphql, very similar to a JSON file bunch of key value pairs
                
