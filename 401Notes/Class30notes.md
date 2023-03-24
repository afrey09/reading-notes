Implementation: Hash Tables 

CHEAT SHEET

Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

Hashing - a technique that is used to uniquely identify a specific object from a group of similar objects. 

  Implemented in 2 steps:

      1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
      2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

Hash Function - A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.

Hash table - A hash table is a data structure that is used to store keys/value pairs. It uses a hash function to compute an index into an array in which an element will be inserted or searched. By using a good hash function, hashing can work well. Under reasonable assumptions, the average time required to search for an element in a hash table is O(1).

Separate chaining (open hashing) - one of the most commonly used collision resolution techniques. It is usually implemented using linked lists. In separate chaining, each element of the hash table is a linked list. To store an element in the hash table you must insert it into a specific linked list. If there is any collision (i.e. two different elements have same hash value) then store both the elements in the same linked list.

Applications for Hash Tables:

  Associative arrays: Hash tables are commonly used to implement many types of in-memory tables. They are used to implement associative arrays (arrays whose indices are arbitrary strings or other complicated objects).
  
  Database indexing: Hash tables may also be used as disk-based data structures and database indices (such as in dbm).
  
  Caches: Hash tables can be used to implement caches i.e. auxiliary data tables that are used to speed up the access to data, which is primarily stored in slower media.
  
  Object representation: Several dynamic languages, such as Perl, Python, JavaScript, and Ruby use hash tables to implement objects.
  
  Hash Functions are used in various algorithms to make their computing faster

Methods
  set()
  When adding a new key/value pair to a hashtable:

    send the key to the hash() method.
    
    Once you determine the index of where it should be placed, go to that index
    
    Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
    
    If something does exist, add the new key/value pair to the data structure within that bucket.

  get()
  The get() method takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

  has()
  The has() method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the hash() method and check the hashtable if the key exists in the table given the index returned.

  keys()
  The keys() method returns a collection (array) of unique hash keys.

  hash()
  The hash() method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.

  source:
  https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html

  https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/