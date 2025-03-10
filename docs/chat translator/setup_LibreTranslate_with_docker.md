# Setup LibreTranslate Translation on Local Computer using Docker
<!-- 中文说明：本指南介绍如何使用Docker在本地计算机部署LibreTranslate翻译服务 -->

Yimmenu's chat translation feature relies on LibreTranslate. This guide will help you setup LibreTranslate translation service on your computer.

## Table of Contents
<!-- 目录章节：以下为文档结构导航 -->
 - [Quick Start](#quick-start)
   - [1. Install Docker](#1-install-docker)
   - [2. Run Docker Desktop](#2-run-docker-desktop)
   - [3. Download LibreTranslate Setup Script](#3-download-libretranslate-setup-script)
   - [4. Run Setup Script](#4-run-setup-script)
 - [Advanced](#advanced)
   - [How to Add Startup Arguments](#how-to-add-startup-arguments)
   - [Common Arguments](#common-arguments)
     - [1. Specify Languages to Download](#1-specify-languages-to-download)
     - [2. Specify IP Address Binding](#2-specify-ip-address-binding)
     - [3. Specify Listening Port](#3-specify-listening-port)
 - [Removal](#removal)
    - [Uninstall Docker](#uninstall-docker)
    - [Remove LibreTranslate from Docker](#remove-libretranslate-from-docker)
      - [Using Docker Desktop](#using-docker-desktop)
      - [Using Docker Command](#using-docker-command)
      
## Quick Start

### 1. Install Docker
<!-- 安装步骤：根据操作系统选择对应的Docker安装方式 -->

Windows: [Install Docker on Windows](https://docs.docker.com/desktop/install/windows-install/) \
Linux: [Install Docker on Linux](https://docs.docker.com/desktop/install/linux-install/) \
Mac: [Install Docker on Mac](https://docs.docker.com/desktop/install/mac-install/)

For Windows users, after running the Docker Desktop installer, simply click OK, and the installer will automatically complete all steps. If you haven't enabled WSL in control panel, restart Windows as prompted after installation to use Docker.

![docker_setup](https://github.com/sch-lda/YimMenu/assets/54973190/96b42f4e-dedc-4ba8-96af-496490325f0a)
<!-- 图示说明：Docker安装界面示意图 -->
![docker_setup_restart](https://github.com/sch-lda/YimMenu/assets/54973190/728842f0-b364-4ad6-ab24-302967fbc4db)

### 2. Run Docker Desktop
<!-- 操作说明：启动Docker Desktop并完成初始化配置 -->

You must run Docker Desktop and complete the initialization configuration before proceeding.

Open Docker Desktop from the desktop shortcut or start menu \
Click `Accept` to agree to Docker Desktop's Terms of Service \
Click `Continue without signing in` and then `skip survey`

You can proceed to the next step when you see the green "Engine Running" indicator at the bottom left of the Docker Desktop main window.

![docker_running](https://github.com/sch-lda/YimMenu/assets/54973190/eb7f7e7e-2e05-431d-9bfa-5f7048cff588)

### 3. Download LibreTranslate Setup Script
<!-- 文件下载：根据操作系统选择对应的脚本文件 -->

Windows: [Download run.bat](https://raw.githubusercontent.com/LibreTranslate/LibreTranslate/main/run.bat) \
Linux/Mac: [Download run.sh](https://raw.githubusercontent.com/LibreTranslate/LibreTranslate/main/run.sh)

### 4. Run Setup Script
<!-- 执行脚本：运行脚本自动下载所需镜像和语言模型 -->

Running the script will automatically download LibreTranslate images and all supported languages. This process may take a few minutes.

When the console outputs `Running on http://*:5000`, it means LibreTranslate has successfully run on port 5000. You can now turn on the chat translation switch in Yimmenu and configure the target language.

To stop LibreTranslate, press Ctrl+C in the command prompt window.

After completing the initial installation, to start LibreTranslate, you only need to open Docker Desktop and then run the LibreTranslate setup script.

## Advanced
<!-- 高级配置：自定义安装参数和运行设置 -->

### How to Add Startup Arguments
<!-- 参数说明：通过命令行参数自定义服务配置 -->

Open Command Prompt or Linux Shell and use the `cd` command to navigate to the directory where `run.bat` or `run.sh` is located. For example, if your `run.bat` file is in `E:\git-repo\LibreTranslate\run.bat`, you need to use the command `cd /d "E:\git-repo\LibreTranslate"`.

Run with additional arguments:

Linux/macOS: `./run.sh [args]` \
Windows: `run.bat [args]`

LibreTranslate supports various parameters, see [here](https://github.com/LibreTranslate/LibreTranslate?tab=readme-ov-file#arguments) for details.

### Common Arguments
<!-- 常用参数：列举最可能用到的配置参数 -->

This document only lists the most likely parameters to be used as the backend service for Yimmenu chat translation.

#### 1. Specify Languages to Download
<!-- 语言选择：限制下载的语言模型以节省空间 -->

If you don't want the translation models to take up too much space, you can add parameters to specify which models to load. See the full language support list [here](https://www.argosopentech.com/argospm/index/). 

For example, if you only need Chinese-English translation, you can use the command `run.bat --load-only zh,en --update-models`.

#### 2. Specify IP Address Binding
<!-- 网络配置：设置服务绑定的IP地址 -->

If you don't want the LibreTranslate translation service to be exposed to networks outside your local computer, you can use `--host [ip]` to modify the IP address bound by LibreTranslate. When set to 127.0.0.1, other computers on the LAN will be unable to access LibreTranslate service on your computer. 

For example, `run.bat --host 127.0.0.1`.

#### 3. Specify Listening Port
<!-- 端口设置：修改服务监听端口号 -->

If other programs need to use port 5000, you can use the `--port [port]` parameter to customize the listening port of LibreTranslate. 

For example, `run.bat --port 8080`.

**If you change the listening port of LibreTranslate, please fill in the same port in the URL setting of Yimmenu chat translation settings.**

## Removal
<!-- 卸载指南：如何移除Docker和LibreTranslate -->

### Uninstall Docker
<!-- 完全卸载：移除Docker及其所有组件 -->

If your Docker is only used to run LibreTranslate, you can uninstall Docker directly from the control panel or Windows settings after stopping LibreTranslate, and LibreTranslate will be completely removed as well.

### Remove LibreTranslate from Docker
<!-- 部分卸载：仅移除LibreTranslate相关组件 -->

If you wish to uninstall LibreTranslate while keeping other containers, please follow this guide.

#### Using Docker Desktop
<!-- 图形界面：通过Docker Desktop进行卸载操作 -->

You can easily remove all images and volumes of LibreTranslate using the GUI of Docker Desktop. Please ensure that LibreTranslate is not running.

![docker_uninstall_volumes](https://github.com/sch-lda/YimMenu/assets/54973190/bb1201dc-1fb9-4208-bda7-2dc61ac59355)
![docker_uninstall_images](https://github.com/sch-lda/YimMenu/assets/54973190/0ca02c98-a008-49db-9cf1-f36dec88c9fc)

#### Using Docker Command
<!-- 命令行：使用docker命令进行卸载操作 -->

If you are using Docker Engine for Linux/Mac, you can also remove LibreTranslate using docker command:

```bash
docker image rm libretranslate/libretranslate
docker volume rm lt-db
docker volume rm lt-local
```
