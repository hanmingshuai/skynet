## skynet_main.c   
main函数其实就是，解析配置，做一些初始化，然后使用配置去调用启动函数。
## skynet_start.c
skynet_start做的就是继续初始化，这里需要注意的是bootstrap，这里通过配置可以知道，其实是启动的是snlua（用C写的模块），之后所有的lua服务都是通过snlua启动的（snlua加载lua文件））先记着，之后再分析。