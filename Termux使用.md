### 第一步：创建 tmux 会话并启动脚本

在 Termux 里执行：

bash

# 创建一个名为 netlogin 的后台会话，并在其中运行脚本
tmux new -s netlogin ~/campus-login.sh

执行后，你会看到脚本开始在 tmux 窗口内滚动输出日志。

---

### 第二步：分离会话（让它在后台跑）

在 tmux 窗口内，按下组合键：

text

Ctrl + b  然后松开，再按 d

你会看到提示 `[detached]`，并退回到普通的 Termux 命令行界面。此时脚本已经在后台持续运行了，**关闭 Termux 应用甚至息屏都不会中断**（前提是你已按之前的方法关闭了电池优化并执行了 `termux-wake-lock`）。

---

### 第三步：以后如何查看运行状态

如果想再次查看脚本的输出日志，重新连接到后台会话：

bash

tmux attach -t netlogin

在查看状态下，按 `Ctrl + b` 再按 `d` 可以再次分离。



### 启动文件服务
1. 根据 `find` 命令的输出，您之前所在的 `filebrowser` 目录完整路径是：

text

/data/data/com.termux/files/home/.local/opt/filebrowser

要回到那里，直接执行：

bash

cd /data/data/com.termux/files/home/.local/opt/filebrowser

 2. mux new -s filebrowser
./filebrowser

用户账号：admin
密码：admin123456789

## SSH登录密码
u0_a308
密码：000000
# 连接手机：

## ssh -p 8022 u0_a308@100.102.52.69


