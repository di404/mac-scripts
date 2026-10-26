# mac-scripts

macOS 实用脚本合集。

| 工具 | 作用 |
| --- | --- |
| [lid](lid/) | 切换合盖后是否待机 |
| [cleanlock](cleanlock/) | 锁定键盘和触控板，方便清洁 |

## 安装

```bash
git clone https://github.com/di404/mac-scripts.git ~/mac-scripts
mkdir -p ~/.local/bin
ln -s ~/mac-scripts/lid/lid ~/mac-scripts/cleanlock/cleanlock ~/.local/bin/
```

确保 `~/.local/bin` 在 `PATH` 中。

## lid

```bash
lid          # 切换
lid on       # 合盖不待机
lid off      # 合盖待机（系统默认）
lid status   # 查看当前状态
```

需要输入管理员密码。

## cleanlock

```bash
cleanlock      # 锁定，10 分钟后自动解锁
cleanlock 5    # 锁定，5 分钟后自动解锁
```

连续按 8 下 `F` 解锁。

首次使用需在「系统设置 → 隐私与安全性 → 辅助功能」中允许你的终端 App。需要 Xcode 命令行工具（`xcode-select --install`），首次运行会自动编译。
