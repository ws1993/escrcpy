<div style="display:flex;">
  <img src="./electron/resources/build/logo.png" alt="viarotel-escrcpy" style="width: 108px;">
</div>

# Escrcpy

📱 使用图形界面的 Scrcpy 显示和控制您的 Android 设备，由 Electron 驱动。[English Document](https://github.com/viarotel-org/escrcpy/blob/main/README.md)

<div style="display:flex;">
  <img src="./screenshots/zh-CN/overview.jpg" alt="viarotel-escrcpy" style="width: 100%;">
</div>

[更多截图](https://github.com/viarotel-org/escrcpy/tree/main/screenshots/zh-CN)

## 特点

- 🏃 同步：得益于 Web 技术，将更快速的与 Scrcpy 保持同步
- 🤖 自动化：允许自动连接到历史设备并自动执行镜像。
- 💡 定制化：支持对多个设备偏好进行独立配置，并且能够添加备注以及导入导出所有配置的功能
- 🔗 反向供网：集成了 Gnirehtet 反向供网功能
- 🎨 主题：支持浅色模式和深色模式，跟随系统切换
- 😎 轻巧度：本机支持，仅显示设备屏幕
- ⚡️ 性能：30~120 帧每秒，取决于设备
- 🌟 质量：1920×1080 或更高
- 🕒 低延迟：35~70 毫秒
- 🚀 快速启动：显示第一张图片仅需约 1 秒钟
- 🙅‍♂️ 非侵入性：不会在安卓设备上留下任何安装文件
- 🤩 用户收益：无需账户、无广告、无需互联网连接
- 🗽 自由：免费且开源软件

## 获取软件包

[查看发布地址](https://github.com/viarotel-org/escrcpy/releases)

## 快速上手

### USB 连接

> 注意：如果手机上提示调试授权请点击允许

1. 安卓手机需开启开发者模式并打开 USB 调试
2. 打开 Escrcpy 并将安卓手机连接到你的电脑
3. 这时 Escrcpy 设备列表应该已经检测到你的手机，点击开始镜像
4. 开始享受吧

### WIFI 连接

> 注意：如果首次无线连接失败，你可能需要无线配对请参阅 [常见问题](#常见问题)
>
> 注意：需同时开启无线调试功能，并在无线调试页面中获取你的当前设备的无线地址（通常为你连接 WIFI 时分配的 IP 地址）及端口号（默认为 5555）

1. 同 USB 连接中的 1-2 步骤
2. 将获取到的设备 IP 地址及端口号填写到 Escrcpy 中，然后点击连接设备
3. 这时 Escrcpy 设备列表应该已经检测到你的手机，点击开始镜像
4. 开始享受吧

### macOS && Linux

> 注意：这些平台没有集成 [Scrcpy](https://github.com/Genymobile/scrcpy) 需要手动安装

1. Linux 可参阅的 [安装文档](https://github.com/Genymobile/scrcpy/blob/master/doc/linux.md)
2. macOS 可参阅的 [安装文档](https://github.com/Genymobile/scrcpy/blob/master/doc/macos.md)
3. 安装上述依赖成功后步骤同 USB 连接 和 WIFI 连接

### Gnirehtet 反向供网

> 注意: macOS 内部没有集成如需使用需要手动安装 [安装文档](https://github.com/Genymobile/gnirehtet)

Windows 及 Linux 端内部集成了 Gnirehtet， 用于提供 PC 到安卓设备的反向供网功能。

## 快捷键

请参阅 [scrcpy/doc/shortcuts](https://github.com/Genymobile/scrcpy/blob/master/doc/shortcuts.md)

## 设备操作

### 控制模式

- 镜像
- 录制
- OTG
- 摄像

### 设备交互栏

- 切换键
- 主屏幕
- 返回键
- 通知栏
- 电源键
- 旋转屏幕
- 音量控制
- 截取屏幕
- 重启设备
- 安装应用
- 文件管理
- 反向供网（Gnirehtet）
- 多屏协同

## 偏好设置

> 持续完善中 目前支持以下常用配置

### 通用

- 更换主题
- 调整语言
- 文件存储路径（音视频录制及设备截图都保存在这里）
- Adb 路径
- Scrcpy 路径
- Gnirehtet 路径
- Scrcpy 参数
- 自动连接历史设备
- Gnirehtet 修复
- 开启调试

### 视频控制

- 最大尺寸
- 视频比特率
- 刷新率
- 视频编码
- 显示方向
- 屏幕裁剪
- 显示器
- 视频缓冲
- 接收器(v4l2)缓冲

### 设备控制

- 展示触摸点
- 保持唤醒
- 控制时关闭屏幕
- 控制结束关闭屏幕
- 控制时禁用自动亮屏
- 模拟辅助显示器

### 窗口控制

- 窗口宽度
- 窗口高度
- 窗口横坐标
- 窗口纵坐标
- 无边框模式
- 全屏模式
- 始终位于顶部
- 禁用屏幕保护

### 音频控制

- 音频源
- 音频编码
- 音频比特率
- 音频缓冲
- 音频输出缓冲

### 音视频录制

- 录制视频格式
- 录制视频方向
- 录制时长
- 禁用视频录制
- 禁用音频录制
- 禁用视频播放
- 禁用音频播放

### 输入控制

- 鼠标模式
- 键盘模式
- 键盘注入方式

### 摄像控制

- 启用摄像
- 摄像源
- 摄像尺寸
- 摄像比例
- 摄像帧率

## 下一步做什么？

> 优先级从高到低

1. 用户界面进行优化，制作合适的 Logo ✅
2. 内置的软件更新功能 ✅
3. 录制和保存音视频 ✅
4. 添加设备快捷交互控制栏 ✅
5. 支持自定义 Adb 及 Scrcpy 依赖 ✅
6. 支持自定义设备名称，以及偏好设置的导出及导入 ✅
7. 定制化，支持对单个设备进行独立配置 ✅
8. 添加 macOS 及 linux 操作系统的支持 ✅
9. 支持国际化 ✅
10. 对深色模式的支持 ✅
11. 添加 Gnirehtet 反向供网功能 ✅
12. 添加新的相机镜像相关功能 ✅
13. 更好的多屏协同 ✅
14. 设备交互栏添加更多功能：文件推送、旋转屏幕、音频控制等功能 ✅
15. 支持批量连接历史设备功能 ✅
16. 支持使用内置终端执行自定义命令 ✅
17. 支持设备自动执行镜像 ✅
18. 添加文件传输助手功能 🚧
19. 支持通过界面从设备下载选中的文件 🚧
20. 支持对设备进行分组，以及按组进行批量操作 🚧
21. 添加对游戏的增强功能，如游戏键位映射 🚧

## 常见问题

### 电脑连接设备后无法检测到

1. 请重新插拔你的设备，并确认设备同意了 USB 调试授权窗口。
2. 如果还不行，你的电脑可能缺少必要的驱动程序，请使用第三方工具 如：驱动精灵，安装必要的驱动后重试。

### 无法输入中文

该问题是已知的， Scrcpy 似乎并未直接对中文输入进行测试和支持 需要在手机端安装第三方输入法 以下输入法经测试可以很好支持

- 搜狗输入法
- QQ 输入法
- 谷歌拼音输入法
- Gboard

### 无线连接提示： 目标计算机积极拒绝访问

第一次无线连接可能需要配对 或 插入 USB 以保证与电脑建立连接即授权成功后方可使用

### 通过数据线连接后点击无线模式没有反应

请再点一次，或点击刷新设备，一般不会超过两次，如果还不行，请提供机型和安卓版本信息到 [Issues](https://github.com/viarotel-org/escrcpy/issues)

### 设备交互控制栏为什么不设计为自动跟踪吸附的悬浮菜单?

采用悬浮菜单方案不可避免地会增加对 Scrcpy 的耦合性，并增加与 Scrcpy 同步更新的难度。许多类似的 ScrcpyGUI 软件在使用此方案后不得不投入大量精力，最终因更新困难而放弃开发。因此，综合考虑，我们决定采用现有的方案，并期待 Scrcpy 未来能够增加原生交互控制栏的支持。

### 某些设备连接镜像后可以看到画面但是无法操作

> 注意：以小米手机为例，不仅需要开启 USB 调试还需要开启 USB 调试（安全设置）也就是允许通过 USB 调试修改权限或模拟点击的功能

可供参阅的详细说明 [鼠标和键盘不工作的原因](https://github.com/Genymobile/scrcpy/blob/master/FAQ.md#mouse-and-keyboard-do-not-work)

### 下载软件包时提示报毒导致无法正常下载

> 经过反馈，有时在 Windows 环境下，由于软件包没有进行证书签名，可能会被 Windows Defender 误认为有害而导致拦截提示，可以尝试以下解决方法

1. 打开 `Windows 安全中心`。
2. 选择 `病毒和威胁防护`。
3. 在 `病毒和威胁防护设置` 下，点击 `管理设置`。
4. 找到 `实时保护`，如果权限允许，可以尝试点击关闭。如果无法关闭实时保护，请跳过此步骤。
5. 向下滑动页面，找到 `排除项`，点击 `添加或删除排除项`。
6. 添加您下载软件包的文件夹路径作为排除项，即将该文件夹添加到`排除列表`中。

### 获取设备列表失败或开始镜像/录屏报错

> 该问题一般是 `Adb` 或 `Scrcpy` 依赖路径错误导致的，可以尝试以下解决方法

1. 在菜单中选择 `偏好设置`，然后在 `Global 模式` 下点击右上角的 `重置配置`。
2. 接下来，进入 `设备列表` 页面，并尝试重新开启镜像功能。
3. 如果问题仍然存在，请确保您已下载并安装了最新版本的 `Escrcpy`。
4. 按下 `Ctrl` + `Shift` + `I` 进入开发者工具，并查看是否有任何报错信息。
5. 如果有报错，请截图并在 [反馈问题](https://github.com/viarotel-org/escrcpy/issues) 页面中提交您的问题。

### macOS 关闭窗口选择最小化到托盘后顶部右侧状态栏找不到图标

> 这个一般是状态栏图标过多导致无法展示 Escrcpy 的图标 推荐用以下工具解决

- [iBar](https://www.better365.cn/ibar.html)
- [Bartender](https://www.macbartender.com/)

### macOS 安装成功后打开提示文件损坏

> 这个通常是因为软件包本身没有签名导致的，可以尝试以下解决方法

1. 终端中执行 `sudo spctl --master-disable` 以允许任何来源
2. 终端中执行 `sudo xattr -r -d com.apple.quarantine [AppPath]` 以尝试修复提示软件包损坏

### 无法定位程序输入点 DiscardVirtualMemory 于动态链接库 KERNEL32.dll 上。

仅支持 `Windows 10` 及更高版本。

### 音频捕获异常导致镜像失败

> 通常是因为您的计算机缺少音频输出，或者您的 Android 版本过低（Android 11+）。

请尝试通过`偏好设置`中的`禁用音频转发`功能，以解决此问题。

## 获得帮助

> 因为是开源项目 全靠爱发电 所以支持有限 更新节奏不固定
>
> 注意：非 BUG 或计划外的需求，有偿处理；至于金额，根据问题难易程度，你觉得帮助了多少，看着给吧（维护这些项目已经耗费了大量精力，还要免费花时间解答问题就说不过去了吧...所以白嫖的一律不通过。）

- issues: [反馈问题](https://github.com/viarotel-org/escrcpy/issues)
- email: viarotel@qq.com
- weixin: viarotel
- qq: 523469508

## 致谢

该项目的诞生离不开以下开源项目

- [scrcpy](https://github.com/Genymobile/scrcpy)
- [adbkit](https://github.com/DeviceFarmer/adbkit)
- [electron](https://www.electronjs.org/)
- [vue](https://vuejs.org/)
- [gnirehtet](https://github.com/Genymobile/gnirehtet/)

## 支持项目

> 如果该项目帮到你的话，可以请我喝杯咖啡，让我更有精神完善该项目 😛

<div style="display:flex;">
  <img src="./screenshots/zh-CN/viarotel-wepay.jpg" alt="viarotel-wepay" style="width: 30%;">
  <img src="./screenshots/zh-CN/viarotel-alipay.jpg" alt="viarotel-alipay" style="width: 30%;">
  <a href="https://www.paypal.com/paypalme/viarotel" target="_blank" rel="noopener noreferrer">
    <img src="./screenshots/en-US/viarotel-paypal.png" alt="viarotel-paypal" style="width: 30%;">
  </a>
</div>

## 贡献者

感谢他们的所做的一切贡献！

<a href="https://github.com/viarotel-org/escrcpy/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=viarotel-org/escrcpy" alt="contributors" />
</a>

## Star 历史

[![Star History Chart](https://api.star-history.com/svg?repos=viarotel-org/escrcpy&type=Date)](https://star-history.com/#viarotel-org/escrcpy&Date)
