# Hash Table:
 is a data structure that implements an associative array abstract data type, **a structure that can map keys to values.**
  A hash table uses a hash function to compute an index, also called a **hash code**, into an array of buckets or slots, from which the desired value can be found. During lookup, the key is hashed and the resulting hash indicates where the corresponding value is stored.

  Some important terminologies for Hash Table:

  1. Buckets:  is what is contained in each index of the array of the hashtable. Each index is called a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

  2. Collision: is when more than one key gets hashed to the same location of the hashtable.

  **To achieve a good hashing mechanism, It is important to have a good hash function with the following basic requirements:**
  1. Easy to compute: It should be easy to compute and must not become an algorithm in itself.
  2. Uniform distribution: It should provide a uniform distribution across the hash table and should not result in clustering.
  3. Less collisions: Collisions occur when pairs of elements are mapped to the same hash value. These should be avoided.

  ## Three ways to calculate hash table:
  1. Division method: This is the easiest method to create a hash function. The hash function can be described as −
**h(k) = k mod n**
  2. Folding method: Done by dividing the item into equal-size pieces (the last piece may not be of equal size). These pieces are then added together to give the resulting hash value.
  3. Mid square method: s a very good hash function. It involves squaring the value of the key and then extracting the middle r digits as the hash value. The value of r can be decided according to the size of the hash table.


