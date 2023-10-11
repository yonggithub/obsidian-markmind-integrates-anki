# obsidian-markmind-integrates-anki
Fork from [Obsidian-MarkMind v1.8.3](https://github.com/MarkMindCkm/obsidian-markmind/releases/tag/1.8.3) and extend Anki synchronization functionality.

[中文说明](/README.MD)

# Introduction
This project is a simple modification based on the `MarkMindCkm/obsidian-markmind` project, and it initially integrates ANKI synchronization functionality. The purpose of open-sourcing it is to encourage capable individuals to continue maintaining and improving the Anki integration feature.
Once again, thanks to the author of `MarkMindCkm/obsidian-markmind`.

# DEMO
![play](/doc/images/play.gif)

# Installation
- If you have already installed `obsidian-markmind`, please delete the installation file `.obsidian\plugins\obsidian-markmind` to avoid conflicts.
- In the `.obsidian\plugins` directory, create a new folder named `obsidian-markmind` and place these 4 files: `main.js`, `diff.min.js`, `styles.css`, and `manifest.json` inside the `obsidian-markmind` folder.
- Restart Obsidian.

# Usage
- Install [AnkiConnect plugin](https://ankiweb.net/shared/info/2055492159) in Anki. Configure AnkiConnect plugin as follows:
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
- Import the template `anki_model\Default.apkg` into Anki.
- In Obsidian, create a "Mind Map."

![Alt text](/doc/images/image.png)

- Click on the ![Alt text](/doc/images/image-1.png) button on a node, and then click the ![Alt text](/doc/images/y.png) button to sync the card to Anki.

![Alt text](/doc/images/add-card.png)
![Alt text](/doc/images/sync.png)

- Additional features supported include "Batch Sync" and "Diff" operations.

# Disclaimer
If this repository infringes on any rights, please inform us, and we will address the issue promptly.

# Thank You
[MarkMindCkm/obsidian-markmind](https://github.com/MarkMindCkm/obsidian-markmind)

[kpdecker/jsdiff](https://github.com/kpdecker/jsdiff)