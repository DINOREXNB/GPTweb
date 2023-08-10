# GPT_Web
- 一个可与GPT聊天的网页客户端
- 需要APIkey才能使用！
- 前往https://platform.openai.com/account/org-settings 查看你的组织ID
- 前往https://platform.openai.com/account/api-keys 获取你的APIkey
# 功能：
- [x] 自选模型
- [x] 自定义逆天程度 
- [x] 单句回复/连续对话
- [x] 重新生成回复
- [x] 文字生成图片
- [x] 加载预设人格
- [x] 支持markdown渲染
- [ ] 重新编辑发送内容
- [ ] 历史对话存储
# 快速开始
## NodeJS
- 使用npm安装以下模块
```
npm install express querystring body-parser mysql2 js-yaml express-session
```
- 将源代码下载至本地
```
git clone https://github.com/DINOREXNB/GPT_Web.git
```
- 进入工作区后，将`Settings_example.yaml`重命名为`Settings.yaml`，编辑配置文件
```
# 数据库配置信息(optional)
mysql:
 host: 'localhost'
 port: 3306
 user: 'root'
 password: '114514'
 database: 'client'

# 服务器配置(required)
server:
 ip: "localhost"
 port: 1145
 location: "https://example.com"
```
- 启动服务器
```
node server.js
```