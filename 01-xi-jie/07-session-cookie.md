# 会话和小甜饼

## 会话

摘录原话：

`会话支持在 PHP 中是在并发访问时由一个方法来保存某些数据.从而使你能够构建更多的定制程序 从而提高你的 web 网站的吸引力. `

`一个访问者访问你的 web 网站将被分配一个唯一的 id, 就是所谓的会话 id. 这个 id 可以存储在用户端的一个 cookie 中，也可以通过 URL 进行传递. `

## 小甜饼cookie

从文档里面取来的原话:

`PHP 透明地支持 HTTP cookie。cookie 是一种在远程浏览器端储存数据并以此来跟踪和识别用户的机制。可以用 setcookie() 或 setrawcookie() 函数来设置 cookie。cookie 是 HTTP 标头的一部分，因此 setcookie() 函数必须在其它信息被输出到浏览器前调用，这和对 header() 函数的限制类似。可以使用输出缓冲函数来延迟脚本的输出，直到按需要设置好了所有的 cookie 或者其它 HTTP 标头。 `

## 关于这俩货

第一次接触这俩玩意儿的同学，一般都被搞的糊里糊涂。特别是php的处理方式，更让人迷惑。出了设置内容的不同，它都给我们提供了统一的访问方式那就是那两个超全局变量$_COOKIE 和 $_SESSION。但实际上，这两个工作方式完全不同，只是php封装得太好，让我们在使用的时候完全感觉不到过大的差别。