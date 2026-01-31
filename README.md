excalidraw for cf pages

1、从https://github.com/excalidraw/excalidraw下载源码并解压；

2、安装最新版 node.js 搭建编译环境；

3、在源码目录cmd窗口运行 yarn install --ignore-engines ；

4、找到根目录及子项目 excalidraw-app 下的两个 package.json 文件，用记事本打开将"node": "18.0.0 - 22.x.x"改成："node": ">=18.0.0" ；

5、在源码目录cmd窗口运行 yarn build:app 进行编译，会在子目录生成一个 excalidraw-app\build 的文件夹；

6、将 build 文件夹打包成zip文件即可在cf pages上传使用。

