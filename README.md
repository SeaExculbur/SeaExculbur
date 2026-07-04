## Hi，我是 SeaExculbur

电子信息工程大一学生。动手型开发者，底层原理爱好者，独立全栈。

### 在做什么

**[AIChat](https://github.com/SeaExculbur/AIChat)** —— Flask + Vue3 + DeepSeek API 的 AI 聊天平台

- 后端：JWT 鉴权 · SQLAlchemy ORM · SSE 流式响应 · 分页历史记录
- 前端：Vue3 Composition API + Vite + Vue Router（开发中）
- 项目文档：[Plan/](https://github.com/SeaExculbur/AIChat/tree/dev/Plan) 目录整理了 WSGI 协议、Werkzeug 双重身份、Flask context 栈、TCP 握手/挥手、B+ 树索引等底层复盘

在做该项目时，我在 WSGI 协议和 Werkzeug 的双重身份上卡了很久：为什么服务器和应用之间要分两路返回元数据和数据体？Flask 的 app context 栈到底怎么管理请求上下文？为了搞清楚 Response.__call__ 内部做了什么，我一路追到 Werkzeug 源码，看到了它怎么把状态码和响应头交还给服务器、再返回可迭代的响应体。二十年前的WSGI协议的先把头传出去，再传响应体的设计思路，为未来的流式通信奠定了基础。

### 做过的项目

- **MySQL + Python + pyecharts 可视化项目** —— pymysql 操作数据库，pyecharts 出图（GDP 动态柱状图、全国疫情地图），数据采集→存储→展示完整打通，是我第一个综合性较强的项目
- **购物车系统** —— Python + MySQL 增删改查
- **Socket 网络编程** —— TCP/UDP 通信，客户端/服务端模式
- **C 语言数据结构** —— 顺序表全套操作（插入/删除/定位/合并/去重/二分查找），链表学习中
- **装饰器系统训练** —— 29 道练习，覆盖闭包/装饰器工厂/限流/重试/缓存，附带自评文档

### 技术栈

Python · Flask · SQLAlchemy · Vue3 · C · MySQL · Git · pyecharts · MATLAB

### 在学

线性代数（MIT 18.06） · 数据结构与算法 · 机器学习/深度学习

### 关于学习方式与AI协作

我不习惯信任 AI 写的代码，我会拆它的每一行，追到它引用的库，再追到库底层的协议。AI 给我加了"精英保留"算法优化，我做了无数次实验验证它没有存在的必要。AI 建数据库表忘了加索引，我能发现全表扫描的风险并做出修改。AI 是我的参考源，不是我的答案。

### 联系

- 邮箱：3041970456@qq.com
