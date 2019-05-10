# 谷歌云免费科学上网

- 测试洛杉矶机房的连接速度最快为220ms左右，测试地址山东，网络供应商中国移动
- 1：sudo -i 
- 2：wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh && chmod +x shadowsocksR.sh
- 3：./shadowsocksR.sh
    - 输入shadowsocks密码 输入端口号 其他一路回车
    - 保存密码，端口号以防忘记
- 4：设置防火墙规则
    - vpc网络=》防火墙规则=》创建防火墙规则
        - 输入名称
        - 目标选择网络中的所有实例
        - 协议和端口
            - 指定的协议和端口
            - tcp和udp输入刚才指定的端口号
            
- 5：实例重启后就会变更ip       