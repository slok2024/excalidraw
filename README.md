excalidraw for cf pages

1. 项目定位
Excalidraw 是一个虚拟白板工具，专门用于绘制具有手绘风格的图表。它不像 Visio 或 Lucidchart 那样严谨，而是追求一种“草图”感，非常适合用于原型设计、架构草图、流程图或教学演示。

2. 核心特点
手绘美学：所有的线条和形状看起来都像是用笔在纸上画出来的，自带“非正式感”，能让观看者更专注于逻辑而非线条是否绝对对齐。

无限画布：提供一个没有边界的画布，支持缩放和平移。

极简操作：工具栏非常简单（矩形、圆形、箭头、文字等），上手几乎零门槛。

安全与隐私：官方版本支持端到端加密的实时协作，数据通常存储在本地浏览器。

高度集成：支持导出为 PNG、SVG 格式，甚至可以拷贝到剪贴板直接粘贴到 Notion、Obsidian 等笔记软件中。

开发者友好：基于 React 和 TypeScript 开发，提供 NPM 包，方便开发者将其集成到自己的 Web 应用中。

2. 编译过程
1、从https://github.com/excalidraw/excalidraw下载源码并解压；

2、安装最新版 node.js 搭建编译环境；

3、在源码目录cmd窗口运行 yarn install --ignore-engines ；

4、找到根目录及子项目 excalidraw-app 下的两个 package.json 文件，用记事本打开将"node": "18.0.0 - 22.x.x"改成："node": ">=18.0.0" ；

5、在源码目录cmd窗口运行 yarn build:app 进行编译，会在子目录生成一个 excalidraw-app\build 的文件夹；

6、将 build 文件夹打包成zip文件即可在cf pages上传使用。

