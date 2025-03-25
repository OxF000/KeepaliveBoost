# 🔥 KeepAliveBoost
点击star，关注不迷路。

**KeepAliveBoost** 是一个基于开源项目的增强版本。通过 JNI 技术实现进程复活的项目，进一步通过 `ioctl` 提高了复活率，最大程度地增强了应用的持久性。

- **`main` 分支**：利用 `libbinder.so` 与 `ActivityManagerService` 通信的版本。
- **`ioctl` 分支**：使用 `ioctl` 与 binder 驱动通信的版本。

## 快速体验
```bash
# 编译
sh ./gradlew :app:assembleDebug

# 安装
adb install app/build/outputs/apk/debug/app-debug.apk 
```

**项目环境：**

- Kotlin 版本：`1.8.22`
- JDK 版本：`11.0.12`
- Android Gradle 插件版本：`7.4.0`
- Gradle 版本：`7.6`
- 编译 SDK：`33`
- 目标 SDK：`32`
- 最低支持 SDK：`19`

