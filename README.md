# Dota 2 AI Coach · 发布页

这里只放 **Dota 2 AI Coach** 的安装包，同时也是 app 自动更新的来源。源代码在另一个私有仓库，不在这里。

## 下载

到 [Releases](https://github.com/yydxs/dota2-ai-coach-releases/releases/latest) 下载最新版：

- **macOS（Apple 芯片）**：`dota2-ai-coach-<版本>-mac-arm64.dmg`。打开后把 app 拖进「应用程序」，再从「应用程序」里打开。安装包已经过苹果公证，首次打开只会弹系统的标准确认框。
- **Windows 10 / 11（x64）**：`dota2-ai-coach-<版本>-win-x64-setup.exe`。双击即装到当前用户目录，不需要管理员权限。安装包没有代码签名，系统可能弹 SmartScreen；确认来源后选「更多信息 → 仍要运行」。

## 自动更新

装好以后，app 会自己检查这里有没有新版：启动 10 秒后、之后每小时、电脑睡醒时各查一次。有新版就在后台下载，顶栏出现「新版已就绪」，点「重启并更新」就换成新版；不点也行，下次退出 app 时会自动装好。

如果自动更新装不上（比如 app 是直接在 DMG 里打开的），app 会提示「有新版」并带你回到这里下载。

## 校验

每个版本都附带 `SHA256SUMS.txt`，可以用来核对下载的文件有没有损坏或被替换：

```bash
shasum -a 256 -c SHA256SUMS.txt
```

每个版本的 `releases/v<版本>.json` 记录了这个版本所有文件的名称、大小和哈希。
