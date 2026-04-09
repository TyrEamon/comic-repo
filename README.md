# ImageMaster Source Repo

这个仓库目录可以直接作为 `ImageMaster` 的外置源仓库使用。

当前结构：

```text
sources/
  index.json
  *.json
  miru/
    *.json
  scripts/
    *.js
```

导入方式：

1. 把整个目录上传到 GitHub 仓库根目录。
2. 在 `ImageMaster -> Setting -> 源仓库` 里填写：
   - GitHub 仓库地址，例如 `https://github.com/your-name/your-repo`
   - 或直接填写远程 `sources/index.json` 地址
3. 点击“同步源仓库”。
4. 软件会把源下载到本地用户源目录，然后点击“重载本地源”即可生效。

说明：

- `sources/index.json` 决定软件会同步哪些源。
- `sources/scripts/*.js` 是真正可执行的外置源逻辑。
- `sources/miru/` 目前保存的是从 Miru 漫画仓库转换过来的 manifest 素材，后续可以逐个适配成可运行源。
- 当前已经具备实际运行能力的示例包括：
  - `baozi`
  - `jmcomic`
  - `mangadex`
  - `miru/com.dmzj.www.json` + `sources/scripts/dmzj.js`
