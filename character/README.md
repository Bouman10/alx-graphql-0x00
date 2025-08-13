# GraphQuest: Character Queries

This directory contains GraphQL queries and outputs for specific characters from the Rick and Morty API.

## Files overview

Each character ID (1 through 4) includes:

- `character-id-X.graphql`: Query to fetch character by ID.
- `character-id-X-output.json`: Sample JSON response.

---

## GraphQL Endpoint

All queries use this endpoint:

https://rickandmortyapi.com/graphql

---

## Query Format

```graphql
query {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}
Usage
Open character-id-2.graphql, change ID if needed.
Execute in GraphiQL or GraphQL Playground.
Copy the JSON response into the matching output file.
Example Response Structure (abbreviated)
{
  "data": {
    "character": {
      "id": "1",
      "name": "Rick Sanchez",
      "status": "Alive",
      "species": "Human",
      "type": "",
      "gender": "Male"
    }
  }
}
Goal
This setup helps you verify each query executes correctly and outputs are captured as expected.