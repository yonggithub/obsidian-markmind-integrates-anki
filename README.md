# obsidian-markmind-integrates-anki
Fork from [Obsidian-MarkMind v1.8.3](https://github.com/MarkMindCkm/obsidian-markmind/releases/tag/1.8.3) and extend Anki synchronization functionality.

[ENG](/doc/README-EN.MD)

# 介绍
本项目是基于`MarkMindCkm/obsidian-markmind`项目做简单修改, 初步集成了ANKI同步功能. ***开源的目的是希望有能力的人继续维护和完善集成Anki的功能***.
再次感谢`MarkMindCkm/obsidian-markmind`作者.

# 演示
![play](/doc/images/play.gif)

# 安装
- 如果已经安装`obsidian-markmind`, 请先删除安装文件`.obsidian\plugins\obsidian-markmind`,以免冲突
- 在`.obsidian\plugins`目录下新建`obsidian-markmind`文件夹, 将`main.js`,`diff.min.js`,`styles.css`,`manifest.json`这4个文件放进`obsidian-markmind`文件夹中.
- 重启obsidian

# 使用
- Anki 安装[AnkiConnect插件](https://ankiweb.net/shared/info/2055492159), AnkiConnect插件配置如下:
```json
{
    "apiKey": null,
    "apiLogPath": null,
    "ignoreOriginList": [],
    "webBindAddress": "127.0.0.1",
    "webBindPort": 8765,
    "webCorsOriginList": [
        "http://localhost",
        "app://obsidian.md"
    ]
}
```
- Anki 导入模板`anki_model\Default.apkg`
- Obsidian 创建`思维导图`

![Alt text](/doc/images/image.png)
- 在节点上点击![Alt text](/doc/images/image-1.png)按钮.然后点击![Alt text](/doc/images/y.png)按钮同步卡片到Anki.

![Alt text](/doc/images/add-card.png)
![Alt text](/doc/images/sync.png)
- 还支持:`批量同步`, `Diff`等操作.

# 声明
如本仓库侵权请告知,会尽快处理

# 感谢
[MarkMindCkm/obsidian-markmind](https://github.com/MarkMindCkm/obsidian-markmind)
[kpdecker/jsdiff](https://github.com/kpdecker/jsdiff)