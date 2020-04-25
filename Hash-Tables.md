## Hash Tables

- Hash Tables are array-like data structures which store key value pairs
- Their key benefit is allowing O(1) lookup based on these key value pair mappings

#### Hashing

- The key involved is hashed, turning it into an integer
- Hashing a key is deterministic, and will always produce the same integral value
- A good hash method:
  - Get ASCII values of each character
  - Multiply the product by a consistent, preferably large prime
  - Use modulo of the length of the array to get the index
  - Place the key at that index
  
  #### Buckets
  
- Each array index contains buckets, which default to `null`
- Key value pairs are stored in these buckets when they are added

#### Collisions

- Collisions occur when multiple keys are assigned to a single index
- Although a "perfect hash" has no collisions, some amount of collisions is acceptable and manageable
- Collisions can be allowed in a way where their effects are mitigated:
  - Each index contains a Linked List (or Tree)
  - Each key value pair is stored as a node in this sub-structure
  - Any colliding pairs are stored as additional nodes
- Collisions emphasize the importance of storing key value pairs instead of just values, and the functional separation of indeces and keys
