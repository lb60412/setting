# npm 切换源
<pre>
npm config set registry https://r.cnpmjs.org/
// 配置后可通过下面方式来验证是否成功

npm config get registry
// 或npm info express
</pre>


# 使用插件nrm
<pre>
	npm install -g nrm

使用

列出可选的源

nrm ls                                                                                                                                    

* npm ---- https://registry.npmjs.org/
  cnpm --- http://r.cnpmjs.org/
  taobao - http://registry.npm.taobao.org/
  eu ----- http://registry.npmjs.eu/
  au ----- http://registry.npmjs.org.au/
  sl ----- http://npm.strongloop.com/
  nj ----- https://registry.nodejitsu.com/
带 * 的是当前使用的源，上面的输出表明当前源是官方源。

切换

切换到taobao

; nrm use taobao                                                                                                                             

   Registry has been set to: http://registry.npm.taobao.org/
</pre>