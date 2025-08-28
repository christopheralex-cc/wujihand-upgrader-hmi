# Wuji Hand Upgrader

Wuji HMI 应用程序 - 用于机器人灵巧手升级的桌面应用

## 系统要求

- **操作系统**: Linux (Ubuntu 18.04+, Debian 9+, CentOS 7+)
- **架构**: x86_64 (AMD64)
- **依赖**: libtbb2

## 安装方式

### 方式一：AppImage (推荐)

AppImage 是一种便携式应用程序格式，无需安装即可运行。

#### 下载
从以下地址下载最新版本的 AppImage 文件：
- GitHub Releases：https://github.com/christopheralex-cc/wujihand-upgrader-hmi/releases

#### 安装步骤

1. **下载 AppImage 文件**
   ```bash
   wget https://hmi.pan-motor.com/wujihand-upgrader/download/wujihand-upgrader-1.1.0.AppImage
   ```

2. **添加执行权限**
   ```bash
   chmod +x wujihand-upgrader-1.1.0.AppImage
   ```

3. **运行应用程序**
   ```bash
   ./wujihand-upgrader-1.1.0.AppImage
   ```

### 方式二：Debian 包 (.deb)

Debian 包提供系统级安装，适合需要集成到系统菜单的用户。

#### 下载
下载对应版本的 .deb 文件：
- GitHub Releases：https://github.com/christopheralex-cc/wujihand-upgrader-hmi/releases

#### 安装步骤

1. **下载 .deb 文件**
   ```bash
   wget https://hmi.pan-motor.com/wujihand-upgrader/download/wujihand-upgrader_1.1.0_amd64.deb
   ```

2. **安装依赖**
   ```bash
   sudo apt update
   sudo apt install libtbb2
   ```

3. **安装应用程序**
   ```bash
   sudo apt install wujihand-upgrader_1.1.0_amd64.deb
   ```

4. **运行应用程序**
   ```bash
   wujihand-upgrader
   ```

#### 卸载
```bash
sudo apt remove wujihand-upgrader
```

## 版本信息

### 当前版本
- **版本号**: 1.1.0
- **发布日期**: 2025-08-28
- **文件大小**:
  - AppImage: ~150MB
  - Deb: ~95MB

### 更新日志

#### v1.1.0 (2025-08-28)
- 初始版本发布
- 支持 AppImage 和 Debian 包安装
- 集成 Wuji HMI 功能

## 故障排除

### 常见问题

1. **AppImage 无法运行**
   ```bash
   # 检查文件权限
   ls -la wujihand-upgrader-*.AppImage
   
   # 重新添加执行权限
   chmod +x wujihand-upgrader-*.AppImage
   ```

2. **依赖缺失错误**
   ```bash
   # 安装必要的依赖
   sudo apt update
   sudo apt install libtbb2 libtbb-dev -y
   ```
---

**注意**: 首次运行可能需要较长时间来解压和初始化应用程序。请耐心等待。

