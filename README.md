# 需求文档
## 基础功能
- 每个人都可以匿名加入白板、快速创建白板
- 每个白板默认只有一页，但可以添加新页
- 每个人可以在白板某页上创建各类图形，并被其他人实时看到
- 白板有协作模式和只读模式两种，
   -  只有白板的 owner 可以修改模式
   - 只读模式下，每个人都不能编辑，且当前页自动同步
- 图形类型：直线、矩形、椭圆、自由曲线、文本
## 高级功能
- 选中一个图形修改样式，线宽、线性、线色、填充色、字体、字号等。
- 移动、缩放、删除被选中的图形
- 回滚、重做自己的最近编辑的内容（undo、redo）
- 导出白板内容、导入之前的内容
## 拓展功能
- **支持离线模式，在本地画图自行导出、导入**
- **插入html/markdown 富文本内容并实时预览**
- **可插入的图片类型，并可以进行变换**
- **插入附件，生成附件外链**
- **跨平台，支持Android、IOS、macOS、Windows、Linux、Web**

# 演示Demo
- https://www.bilibili.com/video/BV1Wd4y1b7rc/

# 团队分工

## [zhangzqs](https://github.com/zhangzqs)
- 前端json_field_modifier算法模块
- 前端json_diff_patcher算法模块
- 前端json_model_undo_redo算法模块
- 存储数据结构设计
- 通信流程设计
- 前端架构设计与各个图形插件的实现
- 后端代码的基础框架搭建
- 架构文档的编写
- 通信流程图的编写
- 核心算法实现文档的编写
## [jimyag](https://github.com/jimyag)
- 前端json_model_sync算法模块
- 前端矩形/文字图形模块
- 存储数据结构设计
- 通信流程设计
- 后端文件上传模块
- 需求文档的编写
- API接口文档的编写
## [utopiospher](https://github.com/utopiospher)
- 前端Github Action CI脚本的编写
- 部署文档的编写
- 使用说明文档的编写
- 视频DEMO的录制与剪辑

## 参考项目

fluffy是一个在线多人协同白板系统，前端使用flutter编写后端使用rust编写

https://github.com/Y0ngg4n/fluffy_board

https://github.com/Y0ngg4n/fluffy_rest_api

sticker_view是一个可以实现旋转，缩放，平移viewer

https://github.com/gopaldhola99/sticker_view

实现json diff并实现patch
https://github.com/pikaju/dart-json-patch
