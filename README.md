# What is FAST-CDN？
FAST-CDN是一款基于Nginx+lua+redis打造的CDN。基于FAST-CDN进行拓展，可以直接打造成商业化CDN（阿里云CDN、又拍云CDN等厂商80%的功能，FAST-CDN都支持）。适合于准备自建CDN的企业、站长、CDN开发人员参考和学习。FAST-CDN只是商业化CDN的一部分（缓存节点）,自建CDN = DNS智能调度 + 缓存节点 + 管理平台（控制台）。

DNS智能调度可以采用“CloudXns/DNSpod/阿里云解析”等成熟DNS产品，管理平台可以根据自己需求自己开发。

#### 特性
- 基于Nginx+lua+redis开发；lua嵌入到Nginx中用于实现CDN的在线加速业务逻辑;redis用于存储元数据，方便lua实时读取加速域名的配置。
- FAST-CDN 是个二级缓存架构（边缘节点、中心节点），如需做三级缓存，可以自行拓展。
- 缓存用的Nginx第三方模块，nginx_proxy_cache，边缘节点、中心节点的缓存支持集群化。
- FAST-CDN 利用了很多openresty第三方库，比如：lua-resty-dns（DNS解析）、lua-resty-checkups(回源管理)。

#### 功能
一、支持缓存时间配置

	1、按照文件类型设置缓存过期时间；
	2、按照文件目录设置缓存过期时间；
	3、默认缓存策略（需借助动静分离，如果是静态资源，并且状态码处于200-400，则缓存8天；特别的301、302缓存20分钟；）；
二、回源功能

    1、源站设置，源站地址支持IP、域名格式；
	2、回源host设置；
	3、主备源、负载均衡；
三、访问控制

	1、Referer 黑白名单防盗链；
	2、User-Agent黑白名单防盗链；
四、Https配置
	
	1、Http2支持，暂时不支持配置，默认全部支持；
	2、源站SSL证书校验（OSCP功能）；
	3、Https证书配置；
	

# Installation

# Documents

# Version

### Synopsis

# 加入讨论群

