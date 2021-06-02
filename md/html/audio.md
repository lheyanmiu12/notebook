###How to use audio(音频标签)

####属性的使用
|属性|描述|
|:-:|:-:|
|autoplay|加载完成后自动播放|
|controls|音频控制台|
####音频类型支持情况
|类型|描述|
|:-:|:-:|
|.mp3|主流平台都支持|
|.ogg|只有谷歌和火狐支持|
|.wav|除了IE11不支持，其余都支持|
注意：所以，尽可能使用AE、格式工厂等软件进行格式转换。   
注意点：在苹果系列的浏览器和安卓移动端的浏览器全部会禁止自动播放，需要用户点击操作才能播放。

####Example
```
<audio src="media/music.mp3" autoplay controls></audio>
```
#####src   资源source