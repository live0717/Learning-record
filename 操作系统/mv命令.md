---
title: mv命令
date: 2017-03-14 11:23:05
tags:
categories: linux命令
---

### 命令格式

mv [选项] <参数1> <参数2>

### 命令功能

移动文件（或目录）和重命名文件

<!--more-->

### 命令选项

| 选项           | 含义                             |
| ------------ | ------------------------------ |
| `-b`         | 覆盖时，会为其创建一个备份                  |
| `-i`(**推荐**) | 覆盖时，会有交互式提醒                    |
| `-f`         | 覆盖时，不会有任何提醒                    |
| `-u`         | 只有当源文件比目标文件新或者目标文件不存在时，才执行移动操作 |

### 命令参数

| 参数1          | 参数2        | 含义                                   |
| ------------ | ---------- | :----------------------------------- |
| 源文件          | 目标文件       | 在同一目录下，只重命名；否则，移动+重命名                |
| 源文件（可以有多个参数） | 目标目录（必须存在） | 移动源文件到目标目录                           |
| 源目录          | 目标目录       | 在同一目录下 + **目标目录不存在** 重命名；否则，移动到目标目录下 |

以上的**移动**或者**重命名**过程中，如果有文件名重复，则会自动覆盖文件。