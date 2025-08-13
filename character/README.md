# ALX GraphQL Project - Character Queries

This project contains GraphQL queries and their outputs for retrieving character information from the [Rick and Morty GraphQL API](https://rickandmortyapi.com/graphql).

---

## **Task 0: Query a Single Character by ID**

For each character ID (1–4), the query retrieves:

- `id`
- `name`
- `status`
- `image`

### Files:
- `character-id-1.graphql`
- `character-id-1-output.json`
- `character-id-2.graphql`
- `character-id-2-output.json`
- `character-id-3.graphql`
- `character-id-3-output.json`
- `character-id-4.graphql`
- `character-id-4-output.json`

**Example Query (`character-id-1.graphql`):**
```graphql
query {
  character(id: 1) {
    id
    name
    status
    image
  }
}
Task 1: Get a List of All Characters (Paginated)
Using the characters(page: Int) field, queries retrieve characters from pages 1 to 4.
Selected subfields:
id
name
status
image
Files:
characters-page-1.graphql
characters-page-1-output.json
characters-page-2.graphql
characters-page-2-output.json
characters-page-3.graphql
characters-page-3-output.json
characters-page-4.graphql
characters-page-4-output.json
Example Query (characters-page-1.graphql):
query {
  characters(page: 1) {
    results {
      id
      name
      status
      image
    }
  }
}
How to Run the Queries
Open the Rick and Morty GraphQL Playground
Copy the query from the .graphql file into the editor
Click Run Query
Copy the result and save it in the corresponding .json file