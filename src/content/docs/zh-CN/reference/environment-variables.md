---
title: 环境变量
description: Biome 可用的环境变量列表
---

### `BIOME_LOG_PREFIX_NAME`

添加到日志名称的前缀。默认值：`server.log.`

### `BIOME_LOG_PATH`

守护进程日志将保存的目录。

### `BIOME_CONFIG_PATH`

配置文件的路径

### `BIOME_BINARY`

覆盖正在使用的 Biome 二进制文件。这允许您，例如，使用系统范围的 Biome 二进制文件。

如果您未定义此变量，Biome 将自动检测适用于您平台的正确二进制文件。

```
# Nix 派生示例；二进制文件路径来自 "${pkgs.biome}/bin/biome"
BIOME_BINARY=/nix/store/68fyfw1hidsqkal1839whi3nzgvqv4pa-biome-1.0.0/bin/biome npx @biomejs/biome format .
```