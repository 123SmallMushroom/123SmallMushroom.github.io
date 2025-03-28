# 如何更新MineOptimiz
按照游戏内指引下载[更新脚本](https://github.com/MineOptimiz-Team/packwiz-update-script)

将更新脚本复制到游戏目录

运行脚本，即可将[MineOptimiz](https://github.com/MineOptimiz-Team/MineOptimiz-3rd)更新到其频道最新版本

---

> 该更新脚本不支持macOS

---

## 自动更新
使用启动器的“预启动命令”或“游戏启动前执行命令”功能可实现在启动时自动将MineOptimiz更新至其频道最新版本

---

> Warning! 为testing频道的[MineOptimiz](https://github.com/MineOptimiz-Team/MineOptimiz-3rd)设置自动更新可能导致游戏不稳定！如果不了解相关知识请不要这样操作！

---

---

> 除非关闭版本隔离，否则不建议在使用[PCL2](https://github.com/Hex-Dragon/PCL2)([CE](https://github.com/PCL-Community/PCL2-CE))的情况下使用该功能，[PCL2启动器](https://github.com/Hex-Dragon/PCL2)始终会将脚本运行在.minecraft目录下（无论有没有打开版本隔离）

---

示例：

（[MultiMC](https://github.com/MultiMC/Launcher)/[Prism Launcher](https://github.com/PrismLauncher/PrismLauncher)/[HMCL](https://github.com/HMCL-dev/HMCL)适用）

(Windows)
```batch

cmd /c "$INST_MC_DIR\update.bat"

```
(GNU/Linux)
```bash

#需提前授予运行权限
bash "$INST_MC_DIR/update.sh"

```

## 切换频道
在游戏内可点击“MineOptimiz设置 - 关于... - 更新 - 更新整合包 - 切换更新频道”以切换到stable或testing频道

切换频道后，需删除更新脚本(update.bat, get_commitid.ps1, get_tagid.ps1, update.sh)重新下载并使用脚本更新。在执行脚本前，请删除游戏目录下的config\modpack-update-checker与config\fancymenu文件夹
