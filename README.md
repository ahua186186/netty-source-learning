# 基于netty4.1源码详细注释
解读的代码在transport工程
针对客户端、服务端、pipeline、eventloop相关功能模块详细解读、注释。

1.EventLoopGroup分析路径：
NioEventLoopGroup-->MultithreadEventExecutorGroup-->NioEventLoop
-->SingleThreadEventExecutor-->NioEventLoop.run()-->processSelectedKeysselect-->
-->processSelectedKeysOptimized-->processSelectedKey