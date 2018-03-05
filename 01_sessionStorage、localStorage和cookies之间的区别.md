### cookie和session
    1、生命周期
        cookie要是没有设置保存时间，那么cookie会随着会话结束而关闭，即保存在内存中，cookie要是设置了保存时间，那么cookie会在保存时间结束之后自动消失，即此时的cookie保存在硬盘之中
    2、存储大小
        cookie一般为4KB，session没有限制
    3、存储类型
        cookie为字符串，session能支持任何类型
    4、存储位置
        cookie保存在客户端，session保存在服务端
### localStorage和sessionStorage
    1、生命周期
        localStorage:
            生命周期是永久的，关闭页面或浏览器，其数据不会消失。除非主动删除localStorage的数据，否则永远不会消失。
        sessionStorage:
            生命周期是仅在当前会话下有效。并且独立窗口打开的同一个页面，sessionStorage也是不一样的。
    2、存储大小
        localStorage和sessionStorage存储数据大小一般都是 5MB
    3、存储位置
        localStorage和sessionStorage都保存在客户端，不与服务器进行通信
    4、数据存储类型
        localStorage和sessionStorage都是保存字符串类型，比如JSON对象
    5、应用场景
        localStorage 一般用于长期登录，适合长期保存在本地的数据
        sessionStorage 适用于敏感账号的一次性登录
### WebStorage的优点
    1、<strong>存储数据更大</strong>：cookie一般4kb,webStorage一般5MB
    2、<strong>节省网络流量</strong>：由于从本地获取数据，不需要从发生服务器请求，节省网络流量
    3、<strong>更快显示</strong>：从本地获取数据，所以更快
    4、<strong>更安全</strong>：不用发生网络请求，不需担心网络截获，安全性更高