# Hash Tables

> A hash table, also known as hash map, is a data structure that implements a set abstract data type, a structure that can map keys to values. A hash table uses a hash function to compute an index, also called a hash code, into an array of buckets or slots, from which the desired value can be found.

#### Each key is unique and has an associated value.

A hash is the result of an algorithm taking a string and converting it into a value, which is used to determine the index location of the hash table.

#### A hash table is ideal for quick lookups

A properly optimized hash table is ideal for quick lookups because they are able to determine the exact location where our value is stored in O(1) time complexity.

Similarly, a hash table can insert and delete in O(1) time.

##### The inner workings of a hash table center on the hash algorithhm, managing collisions and finding key-value pairs.

**Collisions** result when the hash algorithm resolves to the same array index for different keys.  In this case, more than one key-value pair is stored in that array location.

Hash tables have the following **internal methods**:

- Add
- Find
- Contains
- GetHash

---

### Resources

- [Intro to hash tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- [what is a hash table? video](https://www.youtube.com/watch?v=MfhjkfocRR0)
- [Basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
- [Hash table wiki](https://en.wikipedia.org/wiki/Hash_table)

---

[Back to table of contents](../README.md)
