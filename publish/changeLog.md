从v1.1.0起，我们发布了一个独立版的[数据同步服务](https://github.com/lyswhut/lx-music-sync-server#readme)，如果你有服务器，可以将其部署到服务器上作为私人多端同步服务使用，详情看该项目说明

### 不兼容性变更说明

- 同步功能，该功能不支持与PC端v2.2.0之前的版本使用

### 新增

- 新增聚合搜索，注：由于这个方式需要对各个源的结果进行排序，所以需要以“歌曲名 歌手”的顺序输入（例如：突然的自我 伍佰），否则排序后的结果可能不是你想要的
- 新增歌单搜索功能
- 新增热门搜索显示，默认关闭，需要到设置-搜索设置开启
- 新增搜索历史记录，默认关闭，需要到设置-搜索设置开启
- 启动软件时自动回到上次的界面，例如上次退出软件时在我的收藏，下次启动软件时会自动进入我的收藏
- 新增PC端所拥有的内置皮肤
- 新增界面字体大小设置
- 添加kg源评论图片展示（@helloplhm-qwq）
- 支持kg源搜索列表、排行榜flac hires歌曲类型的显示（@helloplhm-qwq, @Folltoshe）

### 优化（界面/交互/功能）

- 调整了首页的界面布局
- 优化大屏幕下的字体大小及界面布局显示
- 支持wy源flac hires歌曲类型的显示
- 优化列表数据导入导出的性能，现在进行这些操作应该可以一下子完成且不会再冻结UI了
- 支持kg源搜索列表flac hires歌曲类型的显示（@helloplhm-qwq）

### 优化（程序）

- 优化程序启动性能，优化与程序交互的流畅度
- 重构整个程序，重新梳理了程序逻辑，使其更容易扩展及维护，将大部分代码从JavaScript迁移到TypeScript
- 重写配置管理、列表管理功能，使其与PC端同步，更容易复用PC端的代码

### 修复

- 修复使用酷狗码无法打开某些类型的歌单的问题
- 修复tx源某些歌单无法打开的问题

### 其他

- 升级React Native到v0.71.4并启用新架构
