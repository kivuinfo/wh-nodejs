## 一、Webhostmost在Node.js环境搭建vless-ws-tls脚本

Webhostmost新账户目前仅支持Node.js本地环境编辑或者上传文件方式搭建

Webhostmost老账户建议使用Node.js本地环境编辑文件方式搭建，官方已限制curl与wget依赖，目前脚本已不可用

1、UUID=你的uuid PORT=服务器可使用的端口 都是非必填，自动随机，但DOMAIN=已解析在CF的域名 是必填的

2、快捷方式```bash ndjs.sh```，如果想变更uuid、端口、服务器域名，可将变量放在快捷方式前面快速执行

```
wget -N https://raw.githubusercontent.com/yonggekkk/sb-nodejs/main/whm.sh && UUID=你的uuid PORT=服务器可使用的端口 DOMAIN=已解析在CF的域名 bash whm.sh
```

Webhostmost新/老账户，建议使用外部节点保活方式，可使用workers_keep文件进行保活

节点保活及节点信息地址：https://你已解析在CF的域名/你的uuid

账户保活？请注意：Webhostmost免费账户需要每45天登录一次网页界面，过期会删除数据，请留意

-----------------------------------------------------

## 二、Claw.Cloud在Node.js环境搭建vless-ws-tls脚本

填写UUID、端口、域名三个变量再运行脚本，现实一键无交互运行，每次重装后输出节点信息不变

Claw.Cloud专用一键脚本(无交互)：

```
wget -N https://raw.githubusercontent.com/yonggekkk/sb-nodejs/main/app.js && UUID=你的uuid PORT=服务器可使用的端口 DOMAIN=服务器域名 node app.js
```
----------------------------------------------------------
-----------------------------------------------------
-----------------------------------------------------

### 声明：FORK来自：勇哥（https://github.com/yonggekkk/sb-nodejs）
### 声明：所有代码来源于Github社区与ChatGPT的整合 [eooce](https://github.com/eooce/node-ws)
