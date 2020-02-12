# Database

## General 

### Index 

composite index RMDB - b-tree to optimize write 

### Cache 

cache miss 

### Shard

Load Balancer 

Replica Master-Slave Slave will share read; Write ahead log 

Vertical sharding Pro: easy implement and maintainance Con: redundant; need to join 

Horizontal sharding Consistent hashing How to shard \(which key\)? How to maintain global ID Use a global atomic service to increment the id for every new row UUID\(string\) generated by the service 

Bloom Filter A big bit array + multiple hash function true negative, but tolerate false positive  

## SQL

complex query

SQL tuning 

* execution plan 
* index invalidity 

## Redis/Memcached 

cache shared session store data persist

## ElasticSearch

JSON + REST

inverted index to optimize read 

ELK

## MongoDB

document store, schema-less, indexable only one index document\(json\) = row join on write, do not use on read. so read is faster than RMDB
