# alx-graphql-0x00
## Single Episode Query (Replace ID as Needed)
query {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}

query {
  episode(id: 5) {
    id
    name
    air_date
    episode
  }
}

### Multiple Named Queries (Useful for Submission)
query Episode1 {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}

query Episode2 {
  episode(id: 2) {
    id
    name
    air_date
    episode
  }
}

query Episode3 {
  episode(id: 3) {
    id
    name
    air_date
    episode
  }
}

#### Professional Version Using Variables
query GetEpisode($id: ID!) {
  episode(id: $id) {
    id
    name
    air_date
    episode
  }
}

Variables example:
{
  "id": 1
}

