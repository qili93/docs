## [仅参数名不一致]torch.distributed.rpc.rpc_async

### [torch.distributed.rpc.rpc_async](https://pytorch.org/docs/stable/rpc.html#torch.distributed.rpc.rpc_async)

```python
torch.distributed.rpc.rpc_async(to, func, args=None, kwargs=None, timeout=- 1.0)
```

### [paddle.distributed.rpc.rpc_async](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/distributed/rpc/rpc_async_cn.html#rpc-async)

```python
paddle.distributed.rpc.rpc_async(to, fn, args=None, kwargs=None, timeout=- 1)
```

两者功能一致且参数用法一致，仅参数名不同，具体如下：

### 参数映射

| PyTorch | PaddlePaddle | 备注                               |
| ------- | ------------ | ---------------------------------- |
| to      | to           | 目标 worker 的名字。               |
| func    | fn           | 一个可调用的函数，仅参数名不一致。 |
| args    | args         | 函数 fn 的参数。                   |
| kwargs  | kwargs       | 函数 fn 的字典参数。               |
| timeout | timeout      | RPC 调用的超时时间。               |
