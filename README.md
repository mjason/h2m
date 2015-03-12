# 嗯，这是一个很纯洁的项目

## 如何把一个资源的特征码转换为磁力链接

```ruby
require 'open3'

query = "{query}"

if query =~ /rmdown/
  hash = query.split('=')[1][3..-1]
else
  hash = query
end

url = "magnet:?xt=urn:btih:#{hash}"
Open3.popen3( 'pbcopy' ) { |input,_,_| 
  input << url
}
```

## Alfred 插件

－ 上面有得下载
－ 关键字 h2m
－ 其他自己玩吧

## 协议
 DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                   Version 2, December 2004

Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

Everyone is permitted to copy and distribute verbatim or modified
copies of this license document, and changing it is allowed as long
as the name is changed.

           DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
  TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

 0. You just DO WHAT THE FUCK YOU WANT TO.
