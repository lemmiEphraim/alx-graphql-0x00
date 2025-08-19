# Episode Queries

This directory contains GraphQL queries to fetch specific episode details from the Rick and Morty API using episode IDs.

## Files

- `episode-page-1.graphql`: GraphQL query for episode with ID 1
- `characters-page-1-output.json`: Expected JSON output for episode ID 1
- `characters-page-2.graphql`: GraphQL query for episode with ID 2
- `characters-page-2-output.json`: Expected JSON output for episode ID 2
- `characters-page-3.graphql`: GraphQL query for episode with ID 3
- `characters-page-3-output.json`: Expected JSON output for episode ID 3
- `characters-page-4.graphql`: GraphQL query for episode with ID 4
- `characters-page-4-output.json`: Expected JSON output for episode ID 4

## Query Structure

Each query uses the `episode(id: ID!)` field with the following structure:

```graphql
query {
  episode(id: [ID]) {
    id
    name
    air_date
    episode
  }
}