# Database:

**SQL**— Has relational characteristics such as tables and relationships between tables, including primary keys and foreign keys. SQL must have ACID properties.

**NoSQL**—A database that does not have all SQL properties.

**Column-oriented**—Organizes data into columns instead of rows for efficient filtering. Examples are Cassandra and HBase.

**Key-value**—Data is stored as a collection of key-value pairs. Each key corresponds to a disk location via a hashing algorithm. Read performance is good. Keys must be hashable, so they are primitive types and cannot be pointers to objects. Values don’t have this limitation; they can be primitives or pointers. Key-value databases are usually used for caching, employing various techniques like Least Recently Used (LRU). Cache has high performance but does not require high availability (because if the cache is unavailable, the requester can query the original data source). Examples are Memcached and Redis.

**Document**—Can be interpreted as a key-value database where values have no size limits or much larger limits than key-value databases. Values can be in various formats. Text, JSON, or YAML are common. An example is MongoDB.

**Graph**—Designed to efficiently store relationships between entities. Examples are Neo4j, RedisGraph, and Amazon Neptune.

**File storage**—Data stored in files, which can be organized into directories/folders. We can see it as a form of key-value, with path as the key.

**Block storage**—Stores data in evenly sized chunks with unique identifiers. We are unlikely to use block storage in web applications. Block storage is relevant for designing low-level components of other storage systems (such as databases).

**Object storage**—Flatter hierarchy than file storage. Objects are usually accessed with simple HTTP APIs. Writing objects is slow, and objects cannot be modified, so object storage is suited for static data. AWS S3 is a cloud example.