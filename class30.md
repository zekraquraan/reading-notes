# What is a Hashtable?
Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

## Why do we use them?
Hold unique values
Dictionary
Library

### Hashmap Example:
Hash Code Examples
Consider these examples running Seattle neighborhood names as Strings through two different hash functions.

Notice that although "Pioneer Square" and "Alki Beach" have different sum hashes they ultimately resolve to the same bucket index. Their hashes modulo buckets.length (to turn them into legitimate array indexes) are equal and they ultimately collide.

Calculating hashes and indexes by summing the ascii values of each character:

SUM HASHED: Pioneer Square = 1379
SUM HASHED: Alki Beach = 884
SUM HASHED: U District = 955

BUCKET SIZE=99
SUM INDEX: 1379 % 99 = 92
SUM INDEX:  884 % 99 = 92
SUM INDEX:  995 % 99 = 64
Calculating hashes and indexes by multiplying the ascii values of each character:

MULT HASHED: Pioneer Square = 599126016
MULT HASHED: Alki Beach = 1062823936
MULT HASHED: U District = 578867200

BUCKET SIZE=99
MULT INDEX:  599126016 % 99 = 93
MULT INDEX: 1062823936 % 99 = 31
MULT INDEX:  578867200 % 99 = 43


#### Hashing is implemented in two steps:

An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
The element is stored in the hash table where it can be quickly retrieved using hashed key.

hash = hashfunc(key)
index = hash % array_size

In this method, the hash is independent of the array size and it is then reduced to an index (a number between 0 and array_size − 1) by using the modulo operator (%).


[links](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)



An associative array stores a set of (key, value) pairs and allows insertion, deletion, and lookup (search), with the constraint of unique keys. In the hash table implementation of associative arrays, an array 
�
A of length 
�
m is partially filled with 
�
n elements, where 
�
≥
�
m\geq n. A value 
�
x gets stored at an index location 
�
[
ℎ
(
�
)
]
{\displaystyle A[h(x)]}, where 
ℎ
h is a hash function, and 
ℎ
(
�
)
<
�
{\displaystyle h(x)<m}.[7]: 2  Under reasonable assumptions, hash tables have better time complexity bounds on search, delete, and insert operations in comparison to self-balancing binary search trees.[7]: 1 

Hash tables are also commonly used to implement sets, by omitting the stored value for each key and merely tracking whether the key is present.[7]: 1 

Load factor
A load factor 
�\alpha  is a critical statistic of a hash table, and is defined as follows:[1]

load factor
 
(
�
)
=
�
�
,
{\displaystyle {\text{load factor}}\ (\alpha )={\frac {n}{m}},}
where
�
n is the number of entries occupied in the hash table.
�
m is the number of buckets.
The performance of the hash table deteriorates in relation to the load factor 
�\alpha .[7]: 2  Therefore a hash table is resized or rehashed if the load factor 
�\alpha  approaches 1.[9] A table is also resized if the load factor drops below 
�
max
/
4
{\displaystyle \alpha _{\max }/4}.[9] Acceptable figures of load factor 
�\alpha  should range around 0.6 to 0.75.[10][11]: 110 

##  THings i want to know ?
more about hash map