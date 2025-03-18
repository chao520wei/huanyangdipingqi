# AdsPower 浏览器 Local API 接口与 Headless 操作指南

## 核心概念解析

**关键词**：AdsPower 指纹浏览器、Local API、自动化操作、headless、无界面服务

- **Headless**：指通过参数启动“无界面服务”，无需图形界面的浏览器运行模式。
- **API-Key**：用于操作 Local API 接口的身份凭证，每个账号对应一个唯一的 API-Key，支持同一账号在多个设备上同时使用。

## 如何启动无界面服务？

启动 AdsPower 的无界面服务是一个简单高效的过程，只需获取 API-Key 并配合命令行操作即可。以下是详细步骤：

### 一、获取 API-Key

1. 打开 AdsPower 客户端，进入“账号管理 - 设置”页面。
   

2. 在“基础 API 接口”区域，点击“生成 API-Key”。
   

3. 复制生成的 API-Key，妥善保存以备后续使用。
   

### 二、使用命令行启动无界面服务

1. **准备环境**  
   确保已在 AdsPower 主目录中打开命令行工具（CMD 或 Terminal）。  
   - **Windows** 默认路径：`C:\Program Files (x86)\AdsPower`  
   - **MacOS** 默认路径：`/Applications/adsPower.app/Contents/MacOS/Adspower`

2. **输入命令**  
   将复制的 API-Key 填入以下命令中：  
   - **Windows**：  
     
     AdsPower.exe --headless=true --api-key=XXXX --api-port=50325
     
   - **MacOS**：  
     
     /Applications/adsPower.app/Contents/MacOS/Adspower --args --headless=true --api-key=XXXX --api-port=50325
     
   

3. **确认启动**  
   启动成功后，命令行会返回 Local API 地址，如下图所示：  
   

**注意**：启动无界面服务时，可调整参数以满足需求，具体参数参考上述命令示例。

## 有界面服务 VS 无界面服务

- **有界面服务**：同一账号仅限单设备登录，适合常规操作。
- **无界面服务**：支持同一账号多设备同时登录，非常适合需要自动化操作的场景。

如果您希望在一个账号下实现多设备运行自动化任务，推荐使用 headless 模式结合 API-Key 调用 Local API 接口。

## AdsPower 指纹浏览器推荐

AdsPower 指纹浏览器是一款专为多账号运营打造的防关联、防封号神器，致力于解决出海账号矩阵的安全管理问题，目前已通过市面 100% 指纹安全网站检测！

👉 [【限时福利】点击此处或使用邀请码：VIPFreeTrial 即可免费领取 VIP 会员专业功能浏览器环境试用！](https://bit.ly/adspower_free)

## 操作常见问题解答 (FAQ)

### Q1：可以在同一设备上同时启动有界面和无界面服务吗？
**A**：不可以，二者不可同时运行。

### Q2：更换 API-Key 后，旧值启动的服务还能使用吗？
**A**：不能。系统会提示 API-Key 失效。一个账号仅对应一个有效 API-Key，重置后需使用新值重新启动。

### Q3：如何重置 API-Key？
**A**：在“账号管理 - 设置 - 基础 API 接口”中重新生成即可。

### Q4：更换 API-Key 后，能否更新已启动服务的 API-Key？
**A**：不能。需先关闭服务，再用新 API-Key 重启。

### Q5：如何关闭无界面服务？
**A**：在命令行中按 `Ctrl+C`，或直接关闭命令行窗口即可。

## 总结

通过以上步骤，您可以轻松掌握 AdsPower 浏览器的 Local API 接口和 headless 操作方法。无论是提升自动化效率，还是管理多设备账号矩阵，AdsPower 都能为您的业务提供强大支持！