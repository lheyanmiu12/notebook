###图片使用的选择and响应式图片
   
####图片的选择
|图片类型||
|:-:|:-:|
|jpg|不透明图片，体积足够小，适用于网络传输|
|png|透明图片|
|gif|动图，支持透明，256颜色，千万不要用在过多渐变色的场景|
|webp|新一代图片后缀，体积小并支持透明，但暂时只有谷歌支持|

####响应式的图片
响应式的图片标签
默认让图片显示的是HD高清图  （放在img标签中），平板则显示md图片，手机等小型设备则显示ld图片
让浏览器根据屏幕大小，自动选择适合的图片进行展示，提升加载速度，优化用户体验
####Example
```
    <picture>
	    <source srcset="img/LD.jpg" media="(max-width:300px)"/>
	    <source srcset="img/MD.jpg" media="(min-width:301px) and (max-width:599px)"/>
	    <img srcset="img/HD.jpg"/>
    </picture>
```