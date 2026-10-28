# YUE’s Portfolio — GitHub Pages 完整版

这是现有作品集网站的静态导出，无须安装依赖或编译。包含 11 个纸团、7 个项目、项目介绍及全部展板。动画依赖已本地化。

## 上传 GitHub

1. 解压 ZIP，进入解压后的文件夹。直接选中里面的文件与文件夹上传，确保仓库首页能直接看见 index.html。不要只上传 ZIP，也不要把外层文件夹作为仓库里的额外一层。
2. 在仓库选择 Add file → Upload files。可先上传 assets 文件夹，再上传剩余文件及 src、vat、vendor 文件夹，分别提交。文件超过 100 个时分批上传；保留文件夹层级，不要把图片平铺到根目录。
3. 进入 Settings → Pages，Source 选择 Deploy from a branch，Branch 选择 main，文件夹选择 /(root)，保存。若你使用其他分支，就选择实际上传的分支。
4. 等待部署完成，使用 Pages 提供的网址访问。首次进入可能需要等待图片与三维动画数据加载。

## 本地预览

在此文件夹打开终端，运行 `python -m http.server 8000`，浏览器访问 http://localhost:8000。Windows 也可使用 `py -m http.server 8000`。
不要直接双击 index.html；浏览器会限制本地 JSON、模块和模型文件加载。
三维纸团需要浏览器支持 WebGL；不支持时会进入兼容显示模式。

## 文件

- index.html：网站首页、样式、项目详情浏览。
- src/：三维纸团、动画与交互源代码。
- assets/：封面及全部项目展板。
- vat/：三维纸张模型及动画纹理，必须上传。
- vendor/：固定版本的 Three.js、cannon-es 及必要加载器与许可证，必须上传。
- projects.json、descriptions.json：项目资料及介绍。
- REFERENCE-LICENSE：原纸张交互参考代码的 MIT 许可。
- .nojekyll：GitHub Pages 静态文件标记；如果系统隐藏它，可在文件管理器显示隐藏文件后上传。其余资源无需 Jekyll 处理。

## 项目内容

01：6 张；02：5 张；03：5 张；04：2 张；05：1 张；06 设计项目：34 张；07 论文研究：20 张。
保留了纸张正反面、手绘箭头、虚化背景、点击空白返回和详情图片切换；详情页不包含 View full size 选项。

作品内容版权归作者所有。第三方代码按随附许可使用。此包不包含账号凭据或 Sites 后台配置。

官方说明：https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
Pages 设置：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
