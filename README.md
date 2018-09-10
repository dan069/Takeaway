# step-01
## 1. 搭建项目整体界面结构
<img width="200"  src="https://github.com/dan069/Takeaway/blob/master/0.JPG"/>
<img width="200"  src="https://github.com/dan069/Takeaway/blob/master/1.JPG"/>
<img width="200"  src="https://github.com/dan069/Takeaway/blob/master/2.JPG"/>
    stylus的理解和使用
        结构化, 变量, 函数/minxin(混合)
    vue-router的理解和使用
        router-view/router-link/keep-alive
        $router: 路由器对象, 包含一些操作路由的功能函数, 来实现编程式导航(跳转路由)
        $route: 当前路由对象, 一些当前路由信息数据的容器, path/meta/query/params
    项目路由拆分
    底部导航组件: FooterGuide
    导航路由组件: Msite/Search/Order/Profile

## 2. 抽取组件
    头部组件: HeaderTop, 通过slot来实现组件通信标签结构
    商家列表组件: ShopList
    
## 3. 登陆路由组件
     静态组件
     FooterGuide的显示/隐藏: 通过路由的meta
     
## 4. 后台项目
    启动后台项目: 理解前后台分离
    测试后台接口: 使用postman
    修正接口文档

## 5. 前后台交互
    ajax请求库: axios
    ajax请求函数封装: axios + promise
    接口请求函数封装: 每个后台接口


# step-02
## 1. 异步数据
    封装ajax: 
        promise+axios封装ajax请求的函数
        封装每个接口对应的请求函数(能根据接口定义ajax请求函数)
        解决ajax的跨越域问题: 配置代理, 对代理的理解
    vuex编码
        创建所有相关的模块: store/index|state|mutations|actions|getters|mutation-types
        设计state: 从后台获取的数据
        实现actions: 
            定义异步action: async/await
            流程:　发ajax获取数据, commit给mutation
        实现mutations: 给状态赋值
        实现index: 创建store对象
        main.js: 配置store
       		
## 2. 登陆/注册: 界面相关效果
    a. 切换登陆方式
    b. 手机号合法检查
    c. 倒计时效果
    d. 切换显示或隐藏密码
    g. 前台验证提示
   
# step-03
## 1. 完成登陆/注册功能
    1). 2种方式
       手机号/短信验证码登陆
       用户名/密码/图片验证码登陆       
## 2. 搭建商家整体界面
    1). 拆分界面路由
    2). 路由的定义/配置|使用

## 3. 模拟(mock)数据/接口
    1). 前后台分离的理解
    2). mockjs的理解和使用
    3). jons数据设计的理解
     
## 4. 项目优化
    1). 缓存路由组件对象
    2). 路由组件懒加载
    3). 图片司加载: vue-lazyload
    4). 分析打包文件并优化 
