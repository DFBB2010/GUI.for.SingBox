1、下载最新的源码：
https://github.com/GUI-for-Cores/GUI.for.SingBox/releases
https://github.com/GUI-for-Cores/GUI.for.Clash
2、在一台win10或win11电脑安装go和node.js最新版，因为源码要求node不能低于v20+才能编译不出错；https://nodejs.org/zh-cn
3、可根据官方要求安装pnpm和wails等命令及相关依赖，如果出错可以随时问ai来解决；
4、进入源码/frontend的目录下运行cmd命令行并执行 pnpm install --frozen-lockfile && pnpm build 编译好前端；
5、找一台win7系统电脑安装go v1.25魔改版，并安装好npm或是pnpm和wails及依赖；https://github.com/thongtech/go-legacy-win7/releases/
6、拷贝在win10系统编译好的源码整个的拷贝到win7下；
7、通过ai修改main.go相关代码，去掉不支持win7系统的相关特性和动画，防止程序闪退或白屏等；
8、在win7源码根目录中运行cmd并执行 wails build -s -skipfrontend 此命令是跳过前端编译环节，如果出错可以随时问ai来解决；
9、正常会在\build\bin目录中生成exe文件；
10、拷贝支持win7系统的WebView2_Runtime到程序同一个目录中。https://github.com/westinyang/WebView2RuntimeArchive/releases/tag/109.0.1518.78
11、下载win7系统支持的clash和singbox内核。
