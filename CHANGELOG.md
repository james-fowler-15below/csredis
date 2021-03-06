##csredis 2.1.1.0
Added support for Redis 2.8 commands (SCAN, SSCAN, HSCAN, ZSCAN)

##csredis 2.1.0.0
Improved serialization performance
Added support for ISerializable

##csredis 2.0.0.0
Improved handling of pipeline and MULTI/EXEC result parsing.
Breaking change: RedisClient.Multi() returns void instead of string. MULTI server reply may be observed by attaching to TransactionStarted event
RedisClient.StartPipe() now accepts optional boolean indicating whether or not result parsing should occur.
RedisClient.StartPipeTransaction() added to facilitate automatic creation of transaction inside a pipeline.
RedisClient.EndPipe(bool) has no effect and should not be used
RedisClient constructor overloads added to handle default values for port and timeout
TransactionQueuedEventArgs now includes the command and arguments that were queued.

##csredis 1.4.7.1
Fixed bug in tracing for empty stack

##csredis 1.4.7.0
Added tracing

##csredis 1.4.6.0
Better handling of sorted set members in ZREM

##csredis 1.4.5.0
Better handling of sorted set scores in ZADD

##csredis 1.4.4.0
Fix for non-existent hashes now returns null

##csredis 1.4.3.0
Fix for null keys/values in hashes

##csredis 1.4.2.0
Added XML inline documentation

##csredis 1.4.1.0
Added support for extended SET command introduced in Redis 2.6.12

##csredis 1.4.0.0
Added async subscriptions and transactions

##csredis 1.3.0.0
Fixed byte streaming bug in RedisClient

##csredis 1.2.0.0
Fixed bug when reading large amounts of data concurrently

##csredis 1.1.0.0
Added async subscriptions and transactions
