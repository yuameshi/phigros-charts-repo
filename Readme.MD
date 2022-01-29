# 这里是哪里

这里是[Phigros HTML5](https://github.com/HanHan233/phigros-html5)的谱面仓库，用于储存谱面文件

# 提交谱面

在一切的之前，您需要PhiEditor创建的JSON格式谱面或者PEC格式谱面，没有就别说了（

首先`Fork`这个仓库到你的账号，这一步需要一个GitHub账号。如果您没有，只需注册一个，然后 Fork。

首先创建一个具有正确名称的新文件夹，例如 `rrhar` 或 `rrharil` 指的是 `Rrhar'il`。（不要包含特殊字符，如 `' / \ ` 等，不能以.开头）

首先创建一个具有正确名称的新文件夹，例如 `rrhar` 或 `rrharil` 指的是 `Rrhar'il`。（不要包含特殊字符，如 `' / \ ` 等，不能以.开头）

在其中创建或粘贴以下文件
```
meta.json			必须-元数据		(名称不可变更)
base.mp3			必选-音乐		(名称可变更)
chart.json			必须-铺面		(名称可变更)
line.json			可选-判定线贴图	 (名称可变更)
illustration.jpg 	必须-曲绘		 (名称可变更)
```
> 音乐要求：MP3/OGG/WAV等常见格式，大小小于5MB

> 曲绘要求：JPG/PNG等常见格式(WebP没测试过)，大小小于1MB

在`meta.json`内填入歌曲元信息（见下），注意要删除注释，使用英文字符，且双引号需要添加`\`转译。
```javascript
{
	"name":"Spasmodic(Haocore Mix)",	//曲名
	"codename":"sample",				//你的文件夹名称
	"artist":"姜米條-天利",				//曲师
	"musicFile":"SpasmodicSP.ogg",		//音乐文件
	"ezRanking":1,						//EZ定数（可带小数）
	"hdRanking":1,						//HD定数（可带小数,可与上一个相同）
	"inRanking":1,						//IN定数（可带小数,可与上一个相同）
	"atRanking":1,						//AT定数（可带小数,可与上一个相同）
	"lineTexture":"line.json",			//可选-判定线贴图
	"chartEZ":"SpasmodicSP.json",		//EZ谱面（可与上一个相同）
	"chartHD":"SpasmodicSP.json",		//HD谱面（可与上一个相同）
	"chartIN":"SpasmodicSP.json",		//IN谱面（可与上一个相同）
	"chartAT":"SpasmodicSP.json",		//AT谱面（可与上一个相同）
	"chartLegacy":"SpasmodicSP.json",	//Legacy谱面（可与上一个相同）
	"illustration":"SpasmodicSP.png",	//曲绘
	"chartDesigner":"Phigros Spasming Team \"無極病院\"",//谱师
	"illustrator":"笔记RE",				//曲绘制作者
	"sliceAudioStart":"10"				//预览音频切片开始时间（秒），预览音频持续时间为15秒
}
```

完成后，将谱面文件夹（您之前创建的）上传到 *你的Git仓库*（您之前复刻的那个），然后打开一个新的 `Pull Request` 然后等待合并。

# 请最好一次Commit搞定