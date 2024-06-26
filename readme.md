#### mit 6.824 2020
#### 无三方库依赖的raft协议实现

#### 1. mr 简单的mapreduce wordcount 词频统计： go基于csp模型实现的并行任务 mr, main/mrmaster, mrworker, mrsequential 

#### 2. raft 协议实现： raft

#### 3. 基于raft协议的 key-value 键值存储服务： kvraft

#### 4. 键值存储服务的 shard 支持， 切片的复制，基于raft实现的切片同步 shardmaster , shardmaster 

- [x] lab1 mr
- [x] lab2 raft
- [x] lab3 kvraft
- [x] lab4 shardkv
    - [x] challenge1
    - [x] challenge2



##### TODO
- [ ] 优化 if else 减少代码
- [ ] 降低 cpu 使用
- [ ] raft figure8 test 出现过一次 FAIL，需重现
-----

* 2020/03/06 
    整理上传代码
