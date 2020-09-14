# What is FAST-CDN？
FAST-CDN是一款基于Nginx+lua+redis打造的CDN。基于FAST-CDN进行拓展，可以直接打造成国内大厂的商业化CDN，FAST-CDN各个功能也是直接对标阿里CDN、又拍云CDN、Ucloud CDN等。适合各个站长用于自己网站的网页缓存、以及准备自建CDN的同学参考和学习。
- ** 你必须知道的是：FAST-CDN只是商业化CDN的一部分（缓存节点）。一个完整的CDN由三部分组成：DNS调度 + 缓存节点 + 管理平台（控制台）。

#### 特性
    1、基于Nginx+lua+redis开发；lua嵌入到Nginx中用于实现FAST-CDN的业务逻辑;redis用于存储元数据，方便lua实时读取加速域名的配置文件。
    2、FAST-CDN 是个二级缓存架构（边缘节点、中心节点），如需做三级缓存，可以自行拓展。
    3、缓存用的Nginx第三方模块，nginx_proxy_cache，边缘节点、中心节点的缓存支持集群化。
    4、

#### 功能

### 待开发


# Documents

# Version

### Synopsis
