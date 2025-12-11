# alx-graphql-0x00
## One Query Per Character (Most Common)
Character with ID 1
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

Character with ID 2
query {
  character(id: 2) {
    id
    name
    status
    species
    type
    gender
  }
}

Character with ID 3
query {
  character(id: 3) {
    id
    name
    status
    species
    type
    gender
  }
}

Character with ID 4
query {
  character(id: 4) {
    id
    name
    status
    species
    type
    gender
  }
}

### Single Query With Multiple Named Operations
query GetCharacter1 {
  character(id: 1) {
    id
    name
    status
    species
    type
    gender
  }
}

query GetCharacter2 {
  character(id: 2) {
    id
    name
    status
    species
    type
    gender
  }
}

query GetCharacter3 {
  character(id: 3) {
    id
    name
    status
    species
    type
    gender
  }
}

query GetCharacter4 {
  character(id: 4) {
    id
    name
    status
    species
    type
    gender
  }
}

#### Using Variables (Professional Way)
query GetCharacter($id: ID!) {
  character(id: $id) {
    id
    name
    status
    species
    type
    gender
  }
}

Variables example:
{
  "id": 1
}


##### One Query Per Page (Page 1–4)
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

query {
  characters(page: 2) {
    results {
      id
      name
      status
      image
    }
  }
}

query {
  characters(page: 3) {
    results {
      id
      name
      status
      image
    }
  }
}

query {
  characters(page: 4) {
    results {
      id
      name
      status
      image
    }
  }
}

##### Multiple Named Queries in a Single File
query CharactersPage1 {
  characters(page: 1) {
    results {
      id
      name
      status
      image
    }
  }
}

query CharactersPage2 {
  characters(page: 2) {
    results {
      id
      name
      status
      image
    }
  }
}

query CharactersPage3 {
  characters(page: 3) {
    results {
      id
      name
      status
      image
    }
  }
}

query CharactersPage4 {
  characters(page: 4) {
    results {
      id
      name
      status
      image
    }
  }
}

##### Professional Version Using Variables
query GetCharacters($page: Int) {
  characters(page: $page) {
    results {
      id
      name
      status
      image
    }
  }
}

Variables example:
{
  "page": 1
}

