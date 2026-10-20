# Agy Studio

一个承载 Google Antigravity CLI（`agy`）的非官方 Windows 桌面界面，提供项目与聊天侧栏、模型选择、代码/差异审查、网页预览和后台任务。

## 下载

打开本仓库的 **Releases**，选择 **v0.64.0**，在 Assets 中下载：

- `Agy-Studio-0.64.0-Windows-x64-Setup.exe`：推荐的安装版。
- `Agy-Studio-0.64.0-Windows-x64-Portable.zip`：全部解压后运行 `Agy Studio.exe` 的免安装版。
- `SHA256.txt`：下载文件校验值。
- 使用说明：首次安装、登录、网络与数据目录说明。

这是分享试用版本，目标系统为 **Windows 10 / Windows 11，Intel/AMD x64**。不是 macOS、Linux 或 Windows ARM64 原生安装包。

## 第一次使用

1. 安装或完整解压后，打开 Agy Studio。
2. 在配置向导中检测已有 `agy`，或从 Google 官方站点下载安装。
3. 用自己的 Google 账号登录，再选择自己的项目文件夹。

GUI 内置运行时，打开和聊天无需另外安装开发版 Node.js 或 Python。运行具体项目、测试或 Git 功能时，需要该项目所需的工具与依赖。

Google 登录、账号资格、网络和额度仍由 Antigravity 服务决定。分享文件不包含原作者的账号、聊天记录或代理设置。

## 数据与后台任务

默认数据目录为 `%LOCALAPPDATA%\AgyStudio`，不要求存在 E 盘。免安装版也按当前 Windows 用户保存数据；移动程序文件夹不会自动迁移聊天。

关闭窗口会隐藏到托盘，后台任务可以继续。点击 Gemini 托盘图标恢复，需要完全结束时使用托盘菜单中的“退出”。

## 当前验证与限制

已完成 Windows 11 本机的隔离测试，覆盖中文/空格路径、新用户目录、没有额外 Node/Python/Git 的启动、原生终端、模拟 CLI 后台任务、托盘、退出和对话持久化；发行文件进行解包与一致性核验。

尚未在所有 Windows 版本或不同硬件上实机验证。真实 Google 首次安装和账号登录需要接收者在自己的电脑上完成。

已有长测发现 CLI 偶发返回 `ERROR`，以及少量滚动延迟尖峰；完整八小时无异常长测尚未通过。重要修改请保留 Git 或备份，并核对实际差异和测试结果。

安装包未取得代码签名证书，Windows 可能显示“未知发布者”或 SmartScreen 提示。

## 说明

Agy Studio 不是 Google 或 OpenAI 的官方客户端，与两家公司没有隶属关系。Google Antigravity、Gemini 等名称和标识属于其各自权利人。相关服务、CLI 和内置第三方组件适用各自条款及许可。