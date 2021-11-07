# test
学习github用法

# 测试
这里测试是否能够上传到github

# 配置git
命令：  
git config --global user.name "your username"  
git config --global user.email "your email"  
实例：  
git config --global user.name "hugenpwe17"  
git config --global user.email "820029885@qq.com"

# 一些错误的解决方法
// Failed to connect to github.com port 443:connection timed out  
// 查找Internet属性，选择“连接”那个选项，然后再点局域网设置，就可以看到代理端口号和地址  
全局代理：
git config --global http.proxy http://127.0.0.1:7890  
git config --global https.proxy http://127.0.0.1:7890

取消全局代理：  
git config --global --unset http.proxy  
git config --global --unset https.proxy


// Error:OpenSSL SSL_read: Connection was aborted, errno 10053  
git config --global http.sslVerify "false"