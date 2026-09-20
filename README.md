> 这个是Smailr的Chrome插件 https://github.com/EvanTop/smailr-mail-assistant  

# SmailrX

Smailr 邮件助手 Android 应用。由同名 Chrome 扩展迁移而来，支持 API 密钥登录、多账户管理、新邮件提醒、邮件列表与详情、发信/回复、本地隐藏、加密备份等功能。

- 包名：`com.smailr.smailrx`
- 最低支持：Android 8.0（API 26）
- 当前版本：1.2.0

## 功能一览

| 功能 | 说明 |
|------|------|
| API 密钥登录 | 支持 `nm_` 开头密钥，多账户切换与重命名 |
| 新邮件提醒 | 通知栏闪烁 + 角标计数 + 合成提示音 |
| 邮件列表 / 详情 | 支持发信、回复（自动 `Re:` + 原文引用） |
| 本地隐藏 | 每邮箱最多隐藏 500 封，不影响服务端 |
| 加密备份 | PBKDF2-SHA256（210,000 次）+ AES-GCM-256，与原插件互通 |
| 已读状态 | 本机已读确认，跨对账刷新不丢状态 |

## 安装

从 [Releases](https://github.com/EvanTop/smailrx/releases) 页面下载最新 APK 安装。签名为调试证书，可直接覆盖安装。

## 构建

```bash
./gradlew :app:assembleDebug    # 开发版
./gradlew :app:assembleRelease  # 发布版
```

需要 JDK 17 或更高版本。

## 许可

MIT

