CentOS简单快速搭建shadowsocks

开始安装

1、 cd /usr/local/
2、 wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-libev.sh
3、 chmod +x shadowsocks-libev.sh
4、 ./shadowsocks-libev.sh 2>&1 | tee shadowsocks-libev.log

1、设置密码
2、设置端口
3、加密方式
4、按任意键自动安装


查看是否安装成功
ps -ef | grep ss-server | grep -v ps | grep -v grep

其他命令
service shadowsocks start   # 启动
service shadowsocks stop    # 停止
service shadowsocks restart # 重启


需要修改shadowsock配置
vi  /etc/shadowsocks-libev/config.json
{
    "server":["[::0]","0.0.0.0"],
    "server_port":your_server_port,
    "local_address":"127.0.0.1",
    "local_port":1080,
    "password":"your_password",
    "timeout":600,
    "method":"aes-256-cfb"
}




