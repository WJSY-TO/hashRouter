- 链接 带来了页面的互联
- 一切皆资源 链接表示(url)
  重新刷新 坏事? 体验有点差
  <html>
    <head><head>
    <body></body>
  </html>
  全部重新加载
  SPA Simple Page Application(单页面应用程序)
  不再需要像传统一样 全部加载
  ## 路由的做法 vue-router
   单页应用的结构
   不再是n个页面了，一个页面，分为不动的部分和动的部分
   导航 nav a #/page1
   #/page1 path 页面切换的 锚链接
   URL 改变了的事件 container 元素里 DOM
   大型页面 方便跳转
   锚链接让点击链接 不跳转页面成为可能
   可能 #/page1 #开头
   
   路由接管一切  new HashRouter();
   constructor 订阅hashChange事件
  
  新的前端世界在打开 要求新的秩序
  管住所有的路由 #/page hashRouter
  hash => cb() //container 显示;
  class HashRouter
  this.router = {}
  向外提供 register(hash,callback = function(){})
  方法 
  load 
  window.addEventListener('hashchange',this.load.bind(this))
  call,apply es5 手动指定函数内部this的API
  bind this 一样 返回一个新的函数 适合在事件监听时执行
  
  