# Hash Tables
HashTable, it is used to determine the index of the array.

Buckets, it is what is contained in each index of the array of the hashTable.

Collisions, it is what happens when more than one key gets hashed to the same location of the hashTable.

HashTables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value. O(1) time complexity.



- Hash maps do this to store values:

    - accept a key
    - calculate the hash of the key
    - use modulus to convert the hash into an array index
    - store the key with the value by appending both to the end of a linked list

- Hash maps do this to read value:

    - accept a key
    - calculate the hash of the key
    - use modulus to convert the hash into an array index
    - use the array index to access the short LinkedList representing a bucket
    - search through the bucket looking for a node with a key/value pair that matches the key you were given

Internal Methods:
- Add()
- Find()
- Contains()
- GetHash()

***
[Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

[what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)

[basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

[hash table wiki](https://en.wikipedia.org/wiki/Hash_table)