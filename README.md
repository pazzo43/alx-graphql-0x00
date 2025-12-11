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
