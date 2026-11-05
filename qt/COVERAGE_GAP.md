# Qt 专栏覆盖缺口分析

对照四份课程大纲，检查独立仓库 `kemier/qt`（私有）及本仓库是否含 Qt 学习笔记 / 示例代码。

**结论（待私有仓授权后复核）：**

- `kemier/qt` **存在且为私有仓**；本 Cloud Agent 环境只挂载了 `github.com/kemier/2020`，当前 token **无法 clone / API 访问** `kemier/qt`（表现为 404）。
- 在 `kemier/2020` 本树内：无既有 Qt / QML / QSS / FFmpeg / OpenCV 专题内容。
- 因此下列清单暂记为「本环境可见范围内未覆盖」；**不能等价于私有仓实际覆盖率 0%**。把 `github.com/kemier/qt` 加进该 Environment 的 repos 后即可重跑对照。

检查范围（已执行）：`kemier/2020` 全树。相关但非 Qt 的材料（如 `doc/MySQL`）不计为已覆盖。

---

## 总览

| 专栏 | 章节 | 未覆盖节数（约） |
|------|------|------------------|
| 2.x 入门到精通 | 2.1–2.9 | 全部 |
| 3.x 高级进阶 | 3.1–3.4 | 全部 |
| 4.x 项目实战 | 4.1–4.4 | 全部 |
| 5.x 工程师提升 | 5.1–5.4 | 全部 |

---

## 2. Qt 编程入门到精通

### 2.1 开发基础体系 — 未覆盖
- Qt 下载与安装（Windows / Linux）
- Qt Creator
- 信号与槽
- 字符串 / 数据类型 / 容器（QMap、QHash、QVector、QList、QLinkedList）
- QVariant
- 常用算法与正则表达式

### 2.2 常用控件 — 未覆盖
- Layouts & Spacers
- Buttons & Containers
- Item Views / Item Widgets
- Input Widgets / Display Widgets

### 2.3 布局及对话框 — 未覆盖
- QLayout、QStackedWidget、QSplitter、QDockWidget
- 文件 / 颜色 / 字体 / 输入 / 消息 / 自定义对话框

### 2.4 图形 & 模型 & 视图 — 未覆盖
- 绘图与双缓冲
- Graphics View
- Model / View / Delegate

### 2.5 文件操作及事件处理 — 未覆盖
- 读写文件；QFile / QFileInfo / QDir / QTemporaryDir / QTemporaryFile
- 鼠标 / 键盘事件；事件过滤器

### 2.6 服务 / 格式操作 — 未覆盖
- INI / JSON / XML

### 2.7 网络及多线程 — 未覆盖
- Socket API；TCP / UDP 服务端与客户端
- 互斥量、信号量、多线程 C/S
- HTTP；WebSocket

### 2.8 图表 — 未覆盖
- ChartView；曲线 / 折线 / 柱状 / 饼图

### 2.9 QWebEngineView — 未覆盖

---

## 3. Qt 高级进阶

### 3.1 数据库编程 — 未覆盖
- **MySQL**：基础、CRUD、索引、视图、存储过程、触发器、事务、备份恢复、Qt 操作 MySQL
- **SQLite**：安装配置、数据类型、建库建表、CRUD、触发器、索引、视图、事务、Qt 操作 SQLite

### 3.2 Qt OpenCV — 未覆盖
- 环境配置；图像 / 视频读写；QImage / QPixmap / QPainter；相机
- Graphics View（Scene / Item / View）
- 滤波、模板匹配、直方图、MeanShift / CamShift
- 美化、合成、旋转、人脸识别、对比度增强、平滑、边缘检测、傅里叶、霍夫检测

### 3.3 单元测试 — 未覆盖
- QTestLib；数据驱动测试；简单性能测试

### 3.4 打包及发布 — 未覆盖
- Debug / Release；动态库依赖
- InstallShield；Inno Setup

---

## 4. Qt 项目实战

### 4.1 Word 处理软件 — 未覆盖
- 架构与需求分析；窗口框架；文档窗口
- 菜单：文件 / 编辑 / 格式 / 窗口 / 帮助
- 工具栏：新建 / 打开 / 保存 / 另存为 / 打印预览
- 剪贴板；加粗 / 斜体 / 下划线 / 字体颜色；对齐（左 / 右 / 中 / 两端）

### 4.2 QQ 客户端 — 未覆盖
- 登录窗与翻转效果；IP 控件；主界面拖动
- 登录业务；全局类；系统托盘；好友分组
- 聊天窗；头像裁剪；音频；加好友；消息时序
- 群聊；表情 / GIF；文件上传与传输

### 4.3 MP3 播放器 — 未覆盖
- UI 框架；播放列表；本地列表；我的喜欢
- 按名称 / 时长 / 歌手排序；添加 / 删除歌曲
- 皮肤切换；系统托盘

### 4.4 库存管理系统（Qt5 + MySQL） — 未覆盖
- 登录；商品入库；预售订单
- 界面架构；各功能实现；数据备份与恢复

---

## 5. Qt 开发工程师提升

### 5.1 Quick / QML — 未覆盖
- QML 基础（Image / Rectangle / Text / ButtonStyle / Item / BusyIndicator）
- 键盘 / 鼠标 / 定时器 / 触摸事件
- Component & Loader；Anchors / 布局
- 编辑控件；CheckBox / GroupBox / TabView；Canvas（笔刷 / 路径 / 变换 / 裁剪）
- 动画（Property / Number / Color / Path / Spring / Parallel / Sequential / Behavior）
- Model/View（ListView / XmlListModel / TableView / GridView / PathView / Repeater）
- Loader 动态加载；导航视图

### 5.2 QSS — 未覆盖
- 辅助工具与皮肤生成器
- 选择器（类型 / 通配 / 属性 / ID / 类 / 子 / 伪类）
- 常用属性；伪状态与子控件
- 实战：按钮菜单、Radio/Check、LineEdit 自动补全、自定义 ComboBox

### 5.3 核心技术 — 未覆盖
- QtConcurrent（filter / map）
- Phonon；WebKit（API / Engine / Platform）
- QTextDocument 富文本
- QStandardItemModel；QAbstractItemView

### 5.4 FFmpeg + Qt 播放器 — 未覆盖
- 需求分析；主 UI；标题栏；控制栏；播放列表
- 播放器模块设计；消息队列与接口
- stream_open / stream_close；read_thread；Decoder
- 音视频输出；音视频同步

---

## 建议补齐优先级

若从零建 `qt/` 笔记树，建议顺序：

1. **基础主干**：2.1 → 2.2 → 2.3 → 2.5（信号槽、控件、布局、事件）
2. **中级能力**：2.4 → 2.6 → 2.7 → 2.8（MV、文件格式、网络线程、图表）
3. **进阶专题**：3.1 SQLite/MySQL → 3.3 测试 → 3.4 打包
4. **UI 现代化**：5.1 QML → 5.2 QSS
5. **项目落地**（任选）：4.3 MP3 → 4.1 Word → 4.4 库存 → 5.4 FFmpeg 播放器
6. **可选深度**：3.2 OpenCV、4.2 QQ 客户端、5.3 核心框架（Phonon/WebKit 偏历史，可改为 Qt Multimedia / Qt WebEngine）

---

## 目录建议（落地时）

```text
qt/
  README.md
  01-basics/          # 2.1–2.3
  02-graphics-mv/     # 2.4
  03-io-events/       # 2.5–2.6
  04-network-thread/  # 2.7
  05-charts-web/      # 2.8–2.9
  06-database/        # 3.1
  07-opencv/          # 3.2
  08-test-packaging/  # 3.3–3.4
  09-projects/        # 4.x
  10-qml-qss/         # 5.1–5.2
  11-core-ffmpeg/     # 5.3–5.4
  COVERAGE_GAP.md     # 本文件
```
