

## CRUD Rest APIs using Spring boot 2, JPA, Hibernate 2 and MySQL

### Designing RESTful APIs
Following are the important things to consider when designing RESTful API’s:

- While designing any API, the most important thing is to think about the api consumer i.e. the client who is going to use the service. What are his needs? Does the service uri make sense to him? Does the request, response format make sense to him?
- In Rest, we think Nouns (resources) and NOT Verbs (NOT actions). So, URI’s should represent resources. URI’s should be hierarchical and as self descriptive as possible. Prefer plurals.
Always use HTTP Methods.
- GET : Should not update anything. Should be idempotent (same result in multiple calls). Possible Return Codes 200 (OK) + 404 (NOT FOUND) +400 (BAD REQUEST)
- POST : Should create new resource. Ideally return JSON with link to newly created resource. Same return codes as get possible. In addition : Return code 201 (CREATED) is possible.

- PUT : Update a known resource. ex: update client details. Possible Return Codes : 200(OK)

- DELETE : Used to delete a resource.
