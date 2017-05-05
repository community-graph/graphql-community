# GraphQL Community Graph

This is an Graph Database full of activity of the GraphQL community, including

* Twitter
* StackOverflow
* GitHub
* [Meetups]
* [Slack]


## Information

1. Neo4j Database at: http://107.170.69.23:7474/browser, (read-only user: graphql password: graphql)
2. Installed neo4j-graphql extension with [this schema](community-graph.schema) on http://107.170.69.23:7474/graphql/
3. Query against the database with GraphiQL or apollo-client
4. Check out the GraphQL-Community Application (TODO Will)
5. Build an example application

Http-Header for GraphiQL: `Authorization: Basic Z3JhcGhxbDpncmFwaHFs`

Curl Example

```
curl -i -X POST -u "graphql:graphql" -d'{"query": "{ User(name:\"apollographql\") {name}}"}' -H accept:application/json -H content-type:application/json http://107.170.69.23:7474/graphql/
```


## Data Model

### Types 

* User
* Tweet, Tag
* Question, Answer, Tag
* Repository

### Model

![](https://github.com/community-graph/documentation/raw/master/community_graph.png)

### Schema

* [GraphQL Schema IDL](community-graph.schema)

## Queries

* dashboard (followship, activity)
* content discovery (projects, blogs) 
* people activity (over time, when are they falling off)
* channel activity
* identify frequent questions / topics


## Screenshots

![](images/graphql-community-header.jpg)
![](images/graphql-community-introspection.jpg)
![](images/grapiql-simple-query.jpg)
![](images/graphql-community-query-leeb.jpg)
![](images/graphql-community-voyager.jpg)
![](images/graphql.execute.jpg)
![](images/graphql.schema.jpg)
