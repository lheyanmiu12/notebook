###video标签
|属性|描述|
|:-:|:-:|
|video|视频|
|autoplay|自动播放|
|controls|控制台|
####Example
```
<video src="media/video.mp4" autoplay></video>

<video controls>
	<source src="media/video.WebM" type="video/Webm">
	<source src="media/video.mp4" type="video/mp4">
</video>
```
|类型|描述与支持|
|:-:|:-:|
|mp4|MPEG-4/H.264 必须要注意视频编码为H264，否则浏览器会不识别|
|fla|原始不支持|
|ogg|谷歌和火狐支持|
|amw||
|rmvb||
|rm||
|avi||
|WebM|谷歌和火狐和Edge支持|


