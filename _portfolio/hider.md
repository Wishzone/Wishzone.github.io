---
layout: project
title: "Hider"
description: "基于 nRF54L15 与 IMU 的低功耗蓝牙感知设备。"
project_key: hider
permalink: /portfolio/hider/
---

## 项目概述

Hider 将运动检测、蓝牙 HID 交互与设备授权整合在一块自研 PCB 上。设备采用 nRF54L15 与 LSM6DSV16X；固件根据运动状态切换 IMU 的低功耗唤醒与精细采样模式，在确认目标动作后发送预设快捷键。

## 我的工作

- 开发基于 Nordic Connect SDK / Zephyr 的板级固件，完成 IMU 驱动、运动判定、功耗状态切换与 BLE HID 服务。
- 构建设备授权流程，连接固件、浏览器入口与 FastAPI 服务端，并整理工厂登记和维护脚本。
- 通过硬件测试脚本与调试日志检查板级功能，为后续量产验证保留可追溯的测试流程。

## 当前进展

固件和授权服务已有可运行实现；公开量产前仍需继续完成设备级安全配置与生产流程加固。项目源码位于本地工作区，暂不提供公开仓库链接。
