# Data-Structure-and-Algorithm
Try to understand how to use hashset and hashmap in different settings by solving leetcode questions
Hash Table:
What is the principle of hash table?
The key idea of hash table is to use a hash function to map keys to buckets.
1)When we insert a new key, the hash function will decide which bucket the key should be assigned and the key will be stored in the corresponding bucket;
2) when we want to search for a key, the hash table will use the same hash function to find the corresponding bucket and search only in the specific bucket.

Which factors will influence the choice of hash function and collision resolution strategy?

Understand the difference between a hash set and a hash map

How to design a simple version of hash set and a hash map as in a typical standard template library

What’s the complexity of insertion and lookup operations?
Hash Table is a data structure which organizes data using hash functions in order to support quick insertion and search.

Key to design a hash table: the hash function is the most important component of a hash table which is used to map the key to a specific bucket.
The hash function will depend on the range of key values and the number of buckets.

Collision resolution: 
A collision resolution algorithm should solve the following questions:
How to organize the values in the same bucket?
What if too many values are assigned to the same bucket?
How to search a target value in a specific bucket?

These questions are related to the capacity of the bucket and the number of keys which might be mapped into the same bucket according to our hash function.
Let's assume that the bucket, which holds the maximum number of keys, has N keys.
Typically, if N is constant and small, we can simply use an array to store keys in the same bucket. If N is variable or large, we might need to use height-balanced binary search tree instead.
