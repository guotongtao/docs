# nginx内置变量说明

`$arg_PARAMETER` 客户端GET请求中PARAMETER 字段的值

`$args` 客户端请求中的参数

`$binary_remote_addr` 远程地址的二进制表示

`$body_bytes_sent` 已发送的消息体字节数

`$content_length` HTTP请求信息中content-length的字段

`$content_type` 请求信息中content-type字段

`$cookie_COOKIE` 客户端请求中COOKIE头域的值

`$document_root` 针对当前请求的根路径设置值

`$ document_uri`   与$uri相同

`$host` 请求信息中的host头域，如果请求中没有Host行，则等于设置的服务器名

`$http_HEADER`  HTTP请求信息里的HEADER地段

`$ http_host` 与$host相同，但是如果请求信息中没有host行，则可能不同客户端cookie信息

`$http_cookie` 客户端cookie信息

`$http_referer` 客户端是从哪一个地址跳转过来的

`$http_user_agent` 客户端代理信息，也就是你客户端浏览器

`$http_via` 最后一个访问服务器的IP

`$http_x_forwarded_for` 相当于访问网络访问的路径

`$is_args` 如果有args的值，则等于"?"，否则为空

`$limit_rate` 对连接速率的限制

`$nginx_version` 当前Nginx的版本

`$pid` 当前Nginx服务器的进程的进程ID

`$ query_string` 与$args相同

`$remote_addr` 客户端IP地址

`$remote_port` 客户端的端口

`$remote_user` 客户端的用户名，用于 auth basic module验证

`$request` 客户端请求

`$request_body` 客户端发送的报文体

`$request_body_file` 发送后端服务器的本地临时缓存文件的名称

`$request_filename` 当前请求的文件路径名，由root或alias指令与URI请求生成

`$request_method` 请求后端数据的方法，例如"GET",“POST”

`$request_uri` 请求的URI，带参数，不包含主机名

`$ scheme` 所用的协议，如http或者HTTPS，比如rewrite^(.+)$scheme://mysite.namescheme://mysite.namescheme://mysite.nameredirect

`$sent_http_cache_control` 对应http请求头中的Cache-Control，需要打开chrome浏览器，右键检查，选中network，点中其中一个请求的资源

`$sent_http_connection` 对应http请求中的Connection

`$sent_http_content_type` 对应http请求中的Content-Type

`$sent_last_modified` 对应请求中的Last-Modified

`$server_addr` 服务端的地址

`$server_port` 请求到达服务器端口号

`$server_protocol` 请求协议的版本号，HTTP1.0/HTTP1.1

`$uri` 请求的不带请求参数的URI，可能和最初的值有不同，比如经过重定向之类的