## 安装系统:win8_64bit

## 1.安装已经下载好的文件.
  ```git
  自定义安装到D:\Program Files\mongodb目录下
  ```
## 2.配置服务
  ```git
  首先是在D:\Program Files\mongodb下创建一个db的文件夹,作为数据存放地址.
  (D:\Program Files\mongodb\db)
  ```
  ```git
  如果有需要,可以将D:\Program Files\mongodb\bin添加到电脑的环境变量PATH中,
  这样mongodb的命令就是全局变量了,在CMD中可以任意使用
  ```
  ```git
  在CMD中执行 mongod --dbpath "D:\Program Files\mongodb\db"  
  (这里的参数是需要用引号包括起来的 --!)
  ```
  ```git
  命令执行完后,注意查看CMD中的信息,服务是否成功启动.  
  (我笔记本上面安装的大蜘蛛一直拦截服务使用27017端口,导致我一直启动服务失败)
  ```
  ```git
  配置服务参数的方式也可以使用配置文件的形式,将要配置的参数写进一个文件中mongo.config,
  然后执行 mongod --config "mongo.config"
  (但是我昨天尝试的时候,CMD提示无法打开我配置的mongo.log文件,具体原因有待调查)
  ```
## 3.访问"http://localhost:27017/",可以访问页面表示服务启动OK
  ```git
  三世哥提醒mongod是服务端,mongo是客户端,才开始了解自己到底在干嘛. <br>
  ```
  ```git
  有些安装教程是把执行mongo作为判断服务启动是否成功的标准,这一点是不准确的.
  比如我机器上安装的大蜘蛛,后来在我启动完mongod服务后,
  使用mongo连接服务端,结果客户端的连接请求被大蜘蛛拦截了,
  也会提示"访问目标积极拒绝"这样的字样.(以上言论仅仅是我个人认识)
  ```
```git
(昨天在自己的笔记本上面安装mongodb,结果中途出现了很多错误的操作,于是写下来供大家参考.)
```