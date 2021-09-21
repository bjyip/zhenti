## 腾讯前端ieg实习一面凉经
>作者：Jieunsi
>链接：https://www.nowcoder.com/discuss/660265?type=post&order=time&pos=&page=1&ncTraceId=&channel=-1&source_id=search_post_nctrack
>来源：牛客网
时长：50min,平台：腾讯会议+在线文档

### 上来四道题半小时完成
1. 请写出以下代码的输出结果顺序
```
async function async1() {
  console.log('async1 start');
  await async2().then(() => {
    console.log("async2 end!")
  });
  console.log('async1 end');
}
 
async function async2(){
  console.log('async2');
}
 
console.log('script start');
 
setTimeout(function(){
  console.log('setTimeout');
},0)
 
async1();
 
new Promise(function(resolve) {
  console.log('promise1');
  resolve();
}).then(function(){
  console.log('promise2');
})
```

2. 实现5分钟倒计时功能
```
<<!DOCTYPE html>
<html lang="en">
<head>
    <title>Count down</title>
</head>
<body>
<div id="time">5:00</div>
</body>
</html>
```
3. 给定一个数字，按以下规则转换为字符串
[168. Excel表列名称](https://leetcode-cn.com/problems/excel-sheet-column-title/)
4. 根据二叉树创建字符串
[606. 根据二叉树创建字符串](https://leetcode-cn.com/problems/construct-string-from-binary-tree/)

### 其他
1. 树的遍历有哪几种方式
2. 哪一种遍历方式的结果是升序
3. 栈跟队列的区别
4. TCP和UDP的差别
5.  TCP怎么保证传输是准确的
6.  TCP怎么保证数据是完整的
7.  TCP为什么要三次握手
8.  TCP拥塞控制的实现
9.  HTTP的请求方式有哪些
10. GET、POST的区别
11. HTTP响应码
12. HTTPS握手过程
13. 登陆功能怎么实现的
14. 在浏览器存数据有哪些方式
15. localStorage有上限吗
16. 用Vue和用原生JS有什么区别
17. 数据双向绑定
18. 商品搜索功能怎么实现的
19. 有十万条数据，都存在前端，前端如何实现搜索功能
20. 怎么实现像百度一样边输入边搜索
21. 项目中一些比较难的点
22. 最近在学的新东西是什么
23. 反问