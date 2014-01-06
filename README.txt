复制资源文件到工程根目录即可运行.参考http://blog.sina.com.cn/s/blog_74c22b21010173f8.html
注意事项:不支持library工程的打包,需要ant-contrib-1.0b3.jar支持
部分需要修改的关键点:

local.properties中
sdk.dir 指 android adk路径(注意双斜杠)


build.xml中
<!-- 项目名称MapsDemo,可用全局替换为当前项目名称 -->

ant.properties中

application.package=com.example.android.apis 		项目包名
ant.project.name=MapsDemo							项目名(同build.xml)
java.encoding=utf-8									项目编码

out.absolute.dir=									临时文件夹
gos.path=											apk存放文件夹

key.store=											nbtlxx.keystore	签名文件位置
key.store.password=123456							签名密码
key.alias=nbtlxx									签名别名
key.alias.password=123456							别名密码


app_version=1.0										apk版本
market_channels=appchina 							apk渠道(逗号分隔 )
