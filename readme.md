网站由网页构成。超链接串成
web app mobile native app(ios,android)

多页应用 很多页面，会跳转，重新刷新页面
多页应用的缺点
- 用户体验极差：每次点击链接都要等待http请求以及响应，而且是整个页面的刷新，二面白一下
如果传输时间大于0.5秒，会看到明显的白屏
- 相同的HTML片段重复下载
1. preventDefault a
2. herf attribute
3. jquery ajax 发送请求，动态得到html内容
4. p content img src
    $('').src('')

SPA Single Page Application
单页应用

- 页面的状态 可以对应一个路由
SPA 解决了用户体验的问题，但是带来另一个极其严重的问题
浏览记录没有了，
history
如何位每个状态改变，（路由状态），产生一个url(路由)，并且生成一次浏览历史记录
让spa的访问，更像传统的请求，location浏览器地址栏上的操作可以使用了。
如何主动去设置history

- 一个页面对应多个状态，每个页面状态都会有一个route 路由（地址，state数据），又会用来对应一个组件
vue 单页面应用开发，由route响应 匹配相应的组件显示，再一直组件化过程