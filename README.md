# Tmux 配置

个人 tmux 配置。

## 功能特性

- 复制模式使用 Vi 快捷键
- 前缀键：`Ctrl-a`
- 禁用鼠标支持以更好地兼容终端
- 使用 tmux-resurrect 和 tmux-continuum 持久化会话
- 使用 `Ctrl-a + hjkl` 导航窗格
- 支持 Alacritty 终端和 RGB 颜色
- 支持下划线样式（Undercurl）

## 插件

由 [TPM (Tmux 插件管理器)](https://github.com/tmux-plugins/tpm) 管理：

- [tmux-yank](https://github.com/tmux-plugins/tmux-yank) - 复制到系统剪贴板
- [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect) - 持久化 tmux 环境
- [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum) - 自动保存和恢复
- [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) - 在 vim 和 tmux 窗格间无缝导航

## 安装

```bash
# 克隆此仓库
git clone git@github.com:zc1050/tmux.git ~/.config/tmux

# 安装 TPM（如果尚未安装）
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

# 链接 tmux.conf
ln -s ~/.config/tmux/tmux.conf ~/.tmux.conf

# 启动 tmux 并安装插件
tmux
# 在 tmux 内：按 Prefix + I（大写 I）安装插件
```

## 快捷键

| 快捷键 | 功能描述 |
|------------|-------------|
| `Ctrl-a` | 前缀键 |
| `Ctrl-a + a` | 水平分割窗格 (35%) |
| `Ctrl-a + b` | 垂直分割窗格 (45%) |
| `Ctrl-a + c` | 新建窗口 |
| `Ctrl-a + h/j/k/l` | 导航窗格 |
| `Ctrl-a + v` | 在复制模式下开始选择 |
| `Ctrl-a + y` | 复制选中内容到剪贴板 |
| `Ctrl-a + r` | 重新加载 tmux 配置 |
| `Ctrl-a + >/<` | 切换到下一个/上一个会话 |

## License

MIT
