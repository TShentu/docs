# 在 Mac 上安装 Olares

Olares 主要运行于 Linux 系统环境下，同时支持在 macOS 或 Windows 上安装，方便测试和评估使用。

:::info
Mac 版 Olares 目前存在以下限制：
- 不支持分布式存储
- 无法添加本地节点

建议仅用于开发或测试环境。
:::

## 系统要求

Mac 设备需满足以下条件：
- 处理器架构：X86-64 或 ARM64
- 内存：可用内存 8 GB 及以上
- 存储空间：可用磁盘空间 90 GB 及以上
- MacOS 版本：Monterey（12）及以上

## 前置准备

请确保已安装以下软件：
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [MiniKube](https://minikube.sigs.k8s.io/docs/start/?arch=%2Fmacos%2Farm64%2Fstable%2Fhomebrew)
  
  ::: tip
  推荐通过 `homebrew` 安装 minikube。
  :::

## 配置系统环境

1. 打开 Docker Desktop，进入 **Settings** > **Resources**，按以下要求配置资源：
    - **CPU limit**：至少设置为 4 核
    - **Memory limit**：至少设置为 9 GB
    - **Virtual disk limit**：至少设置为 80 GB

   ![更新资源配置示例](/images/manual/get-started/docker-resources-settings.png)

2. 点击 **Apply & restart** 使配置生效。

## 安装 Olares

在终端中运行以下命令：

 ```bash
 curl -fsSL https://cn.olares.sh |  bash -
 ```
:::info 安装遇到报错？
如果安装过程中出现错误，请先执行以下命令卸载：

```bash
bash olares-uninstall.sh
```
卸载完成后，重新运行安装命令进行安装。
:::
## 配置 Wizard
在安装过程最后，你需要提供下列信息：
1. 查看 Mac 的 IP 地址（例如，`192.168.x.x`）。如果自动获取的 IP 地址正确，请按 `Y` 确认。如果需要修改，请按 `R` 并输入正确的地址。
   ::: tip 确认 IP 地址
   要确认 Mac 的 IP 地址，你可以通过图形用户界面（GUI）或命令行（CLI）来完成。

   - **使用 GUI**：打开**系统设置**（或 **系统偏好设置**）> **网络**，查看当前活动网络连接的详细信息。
   - **使用 CLI**：打开一个新的终端窗口，使用 `ipconfig getifaddr en0` （Wi-Fi 连接）或 `ipconfig getifaddr en1`（以太网连接）获取 IP 地址。
   :::
2. 输入在 LarePass 中注册的 Olares ID 前缀。如果你的 Olares ID 为 `alice123@olares.cn`，输入 `alice123` 即可。

   ![Enter domain name and Olares ID](/images/zh/manual/get-started/enter-olares-id.png)

安装完成后，屏幕将显示初始系统信息，包括向导地址和初始一次性密码。这些信息在后续激活步骤中会用到。

![Wizard URL](/images/manual/get-started/wizard-url-and-login-password.png)

## 激活 Olares

使用向导 URL 和初始一次性密码进行激活和 Olares 初始化配置。

1. 在浏览器中输入向导 URL。进入欢迎页面后，按任意键继续。

   ![打开向导](/images/manual/get-started/open-wizard.png)
2. 输入一次性密码，点击**继续**。

   ![输入密码](/images/manual/get-started/wizard-enter-password.png)
3. 选择系统语言。

   ![选择语言](/images/manual/get-started/select-language.png)
4. 使用 LarePass 应用激活 Olares。

   a. 打开 LarePass 应用，点击**扫描二维码**，扫描向导页面上的二维码完成激活。
   :::warning 检查网络连接
   为避免激活失败，请确保你的手机和 Olares 设备连接到同一网络。
   :::
   ![激活 Olares](/images/manual/get-started/activate-olares.png)
   b. 按照 LarePass 上的提示重置 Olares 的登录密码。

设置成功后，LarePass 应用会自动返回主界面，向导页面则会跳转到登录界面。

## 登录流程

1. 在登录页面输入 Olares 登录密码。

   ![登录](/images/manual/get-started/log-in.png)
2. 系统会要求完成双重验证。你可以选择在 LarePass 上确认登录，或手动输入 6 位验证码。
   ::: info
   验证码有时效限制，请在过期前完成输入。如果验证码过期，需要重新生成。
   :::

   ![Confirm login](/images/manual/get-started/confirm-login.png)

登录后你就会看到 Olares 桌面。🎉

## 安全保存 Olares ID
你已经准备好开始使用 Olares！在此之前，请务必确保 Olares ID 已安全备份。如果不备份，你将无法在需要时恢复 Olares ID。

- [备份助记词](./back-up-mnemonics.md)
