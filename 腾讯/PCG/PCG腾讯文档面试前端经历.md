## PCG腾讯文档面试前端经历
### 二面
> 视频面试

1. GET和POST的区别
2. POST参数在请求头还是请求体（我回答请求体
3. 浏览器缓存cookie的控制缓存的属性：maxAge，domain，path
4. 跨域解决方案 CROS JSONP，展开运算符使用场景：解构、做形参
5. Promise的串行怎么实现
6. 比如有100个异步任务怎么实现两两一组执行webPackage打包用过哪些loader
7. loader原理打包时它遇到不认识的文件怎么找对应的
8. loader的loader和plugin有什么区别
9. vue-router用过吗
10. 打包时是怎么把不同router路径的js分别打包到多个trunk里的
11. vue中computed和watch的区别使用场景
12. 设计模式知道吗大四学知道装饰者模式吗不知道
    
## 三面
> 牛客网面试

1. 放松放松别紧张，先介绍一下你自己熟悉一下吧
  我简要概括了几个经历
   1. 和同学俩人外包项目重庆房保宝小程序，房保宝是展示房源信息的，我完成了房保宝的全部前端
   2. 在学校蓝山工作室维护we重邮小程序，we重邮是学校信息平台可以查课表成绩等，我负责每日打卡、离校审批、图书馆可视化等
   3. PC端写过个人博客以及后台管理，部署在了腾讯云服务器
   4. 亚信科技前端实习生，负责联通沃易购PC商场的开发
   5. 希望未来能从事有关前端方面的工作，也希望能在前端这个方面有所升入
2. 我们先看代码题把，后面才是面试
```
2.1 写出javascript运行结果： 
for(var i=0; i<10; i++){} alert(i);
答：10

2.2 写出javascript运行结果：
var a = 1;
function b() {
    var a = 2;
    function c() {
        console.log(a);
    }
    return c;
}
b()();
答：2

2.3 请通过正则替换，把一串字符串两边的分号去掉，
同时把字符串中间连续出现多个的分号变成一个。
如：;ab;;b;;;e;;  --> ab;b;e
提醒你开头结尾的正则使用^  $
开头结尾不会就算了写中间去重吧
答 str.replace(/;+/g,";")

2.4 请手写3种常见的排序算法，以及说出他们的复杂度和运用场景
function bubleSort(arr){//冒泡 log(n^2)
  for(let i=0;i<arr.length-1;i++){
    for(let j=i+1;j<length;j++){
      if(arr[i]>arr[j]){
        let temp=arr[j]
        arr[j]=arr[i]
        arr[i]=temp
      }
    }
  }
  return arr
}

function insertSort(arr){//插入 
  for(let i=1;i<arr.length;i++){
    for(let j=i+1;arr[j-1]<arr[j];j--){
      
      }
    }
}

function getMid(left,right,arr){
  let pvot=arr[right]
  if(arr[left]>pvot&&left<right){
    swrap(arr[left],arr[right])
    right--
  }
  if(arr[right]<pvot&&left<right){
    swrap(arr[left],arr[right])
    left++
  }
  return left
}
function fastSort(left,rigth,arr){//快排
  if(left<rigth){
    let mid=getMid(left,rigth,arr)
    fastSort(left+1,mid-1,arr)
    fastSort(mid+1,rigth-1,arr)
  }
}
function swrap(a,b){
  let temp=a
  a=b
  b=temp
}
```
3. get和post区别
4. http头部有哪些字段
5. 说说tcp三次握手
6. 长连接和短连接的区别
7. webpack打包流程
8. vue的特性
9. react写过吗
10. 闭包有什么作用，为什么要使用闭包，
11. 使用闭包有哪些隐患和缺陷
12. 闭包为什么会出现内存泄露
13. 怎么解决闭包的内存泄露
14. 说说async await的原理
15. display有哪些值
16. inline和inline-block有什么区别
17. css框架用过吗
18. 用less有什么优点
19. 前端学习路线
20. 未来职业规划
21. 为什么选择工作不打算考研呢
22. 你还有什么问题
    
## 评价这次面试表现
面试过程要更严肃一点 代码题有一点是我面过的同学没有的，就是你是第一个主动问我“我记了快排笔记，能不能去看一下” 如果我这边过了后面还有总监面，hr面 我们这边部门是PCG，不是QQ，主要是做效率工具的，腾讯文档等，总部在深圳
评价，知道有解决方案ws，但是不了解原理，我二面虽然没有问你算法数据结构，手撕代码，你肯定准备好了快排，堆排，我问你有什么用呢
其实问你如何快速查询1W条数里面就包含了数据结构、算法，看看你平时如何运用程度到底如何，有没有对项目遇到的问题加以思考

## 四面
1. 介绍自己
2. 我看你也做了许多项目，你项目中遇到的困难的问题是什么？（甲方需要QQ聊天功能）
3. 你怎么解决困难的（查询解决方案，websocket,目前用唤起微信聊天窗口代替）
3. websoket是基于UDP/TCP协议？（TCP）
4. 你简历中写到日访问量2W，怎么知道访问情况的。（微信公众平台后台统计看到的）
5. 学校大概2W人以上，如何更快的查数据（不知道）
6. 查课表、学生信息怎么做到的（接入的是学校的统一认证登录系统）
7. 微信小程序用的什么通讯协议？（不知道）
8. 如何做到更快进入小程序（首页分包加载，附包点击后才加载，空闲时预下载附包）
9. 如何做到预下载附包的呢？
10. 预下载附包不知道，后面分包原理应该不知道我就不问了吧

## 五面
1. 除了专业之外你还有其他兴趣爱好吗
2. 给你自己几个关键词评价自己
3. 说一说你最近接触到了前沿技术
4. 你在前实习生的收货
5. 为什么不考研就业
6. 在项目中负责的功能
7. 你在we重邮或者房保宝最大的贡献
8. 你前端学习路线，为什么报培训班
9. 实习地点的倾向
10. 愿不愿职位城市调剂
11. 你除了腾讯还有没有其他面试
12. 有没有亲戚在腾讯任职
13. 假如你收到了多份offer怎么选择