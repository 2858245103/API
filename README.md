# API【新手用】
-------------------------------------------
自用API，兼容于Node、QuanX环境
------------------------------------------
Node环境需要额外导入：axios ->在终端使用 `npm i axios` 导入模块
--------------------------------------------

const $ = new Env("Demo")
1.发送请求：
异步：
$.http.get(options).then(xxx).catch(xxx)
$.http.post(options).then(xxx).catch(xxx)

回调函数:
$.get(options,(err,res,body)=>{})
$.post(options,(err,res,body)=>{})

其他函数
$.log() = console.log()
$.done() = $done() QuanX环境中需要此函数结束,其他环境无需
$.write() 重写响应
