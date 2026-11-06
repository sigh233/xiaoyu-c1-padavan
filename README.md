# 小娱C1 (XY-C1) Padavan 老毛子固件编译

## 简介
基于 Padavan (老毛子) 源码的小娱C1路由器固件自动编译仓库。

## 功能特性
- 多拨接入 (PPPoE + 静态IP)
- 硬件加速 (NAT Offloading)
- IPv6 支持
- 系统优化
- 固件精简

## 设备信息
- 型号：小娱C1 (XY-C1)
- CPU：MT7620A
- Flash：16MB
- RAM：64MB

## 编译说明
1. 推送代码到 `main` 分支或手动触发 `Workflow Dispatch`
2. CI 自动拉取 Padavan 官方源码
3. 下载依赖工具链
4. 修改系统配置 (开IPv6、关多余服务)
5. 编译并生成 `.bin`/`.trx` 固件
6. 自动上传构建产物到 Release

## 使用方法
在 [Actions](https://github.com/sigh233/xiaoyu-c1-padavan/actions) 页面可以查看编译日志，固件产物会保存在 Actions Artifacts 和 GitHub Releases 中。

## 许可
本项目代码遵循原始 Padavan OpenWrt 许可协议。

## 依赖仓库
- [HanWckf/padavan-4.4](https://github.com/hanwckf/padavan-4.4) - 官方源码库