# 基于netty4.1源码详细注释

针对客户端、服务端、pipeline、eventloop相关功能模块详细解读、注释。

1.注释代码在transport工程中，分析路径：
NioEventLoopGroup-->MultithreadEventExecutorGroup-->NioEventLoop
-->SingleThreadEventExecutor-->NioEventLoop.run()-->processSelectedKeysselect-->
-->processSelectedKeysOptimized-->processSelectedKey