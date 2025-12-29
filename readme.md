
# Typora主题集合（Git Submodule管理）
这是一个Typora编辑器主题的统一管理仓库，通过Git Submodule关联各主题的GitHub源项目，可便捷同步主题更新。


## 仓库克隆
由于包含Submodule，需使用递归克隆拉取所有主题资源：
```bash
git clone --recursive https://github.com/muxuezzz/my_typora_theme.git
```

若克隆后子模块未自动加载，执行以下命令补全：
```bash
git submodule init && git submodule update
```


## 更新主题
将所有主题同步至对应GitHub项目的最新版本：
```bash
git submodule update --remote
```


## 包含的主题列表
| 主题名称               | Submodule路径           | 对应原压缩包             | 源项目地址（替换为实际GitHub链接） |
|------------------------|-------------------------|--------------------------|------------------------------------|
| DrakeTyporaTheme       | DrakeTyporaTheme/       | DrakeTyporaTheme-2.9.6.zip | https://github.com/[作者]/DrakeTyporaTheme |
| typora-ash-theme       | typora-ash-theme/       | typora-ash-theme-master.zip | https://github.com/[作者]/typora-ash-theme |
| typora-theme-phycat    | typora-theme-phycat/    | typora-theme-phycat.zip  | https://github.com/[作者]/typora-theme-phycat |
| Ursine                 | Ursine/                 | Ursine.zip               | https://github.com/[作者]/Ursine   |


## 注意事项
1. 各主题的安装、配置方法，请参考对应Submodule目录内的说明文档；
2. 若需添加新主题，可通过`git submodule add [主题GitHub地址] [本地路径]`命令扩展。


要不要我帮你整理**Typora主题的快速启用步骤指南**？
