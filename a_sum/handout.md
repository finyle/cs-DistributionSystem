## http://nil.csail.mit.edu/6.5840/2023/

# ##############################
## 1. MapReduce 

## intro: paper mapreduce 

## getting started: main/mrsequential, mrapps/wc, mrapps/indexer
## job: mr/coordinator, mr/worker, mr/rpc

## rules: 
## hints: 

## challenge: 
### 1. MapReduce application 
### 2. 基于unix sockets(替换rpc(基于tcp/ip)) 的分布式文件系统


# #############################
## 2. raft

## intro: paper raft

## getting started: raft/raft
## job1: leader election(leader 选举， rpc 请求，响应)
## job2: log (基于日志的 leader 选举)
## job3: persistence (日志持久化： 基于persistent 对象)
## job4: log compaction (snapshot 合并)

## hints: 

# ##############################
## 3. fault-tolerant kv service (基于raft协议的容错kv服务)

## intro: paper raft 

## getting started: kvraft/client, kvraft/server, kvreaft/common
## job1: kv service without snapshot
## job2: kv service with snapshots 

## hints 

# #################################
## 4. sharded kv service 

## intro: 

## getting started: shardctrler/server&client, shardkv/server&client&common

## job1: shard controller 
## job2: sharded kv server 

## challenge(生产环境特性):
### 1. garbage collection of state 
### 2. client requests during configuration changes 


# ################################################################
# src

# 1. main/mrsequential: 
## 注： go buildmode=plugin : windows 环境不支持 plugin 模式， 可以在wsl中编译so文件，再调用

# 2. raft/test_test
## 注：当前目录导包相对路径设置

# 3. kvraft/test_test

# 4. shardkv/test_test
#    shardmaster/test_test

