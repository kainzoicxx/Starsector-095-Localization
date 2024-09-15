﻿# Starsector-0951-Localization

本项目为《远行星号》游戏的中文翻译项目。

目前正在进行的是游戏 **0.95.1a** 版本的汉化，目前进展顺利，主要的剩余任务是对 rules.csv
的校对工作。

## 下载汉化

**注意：本汉化包仅适用于 0.95.1a-RC6 版本**

### 从论坛下载

您可以在论坛帖子 [远行星号 0.95.1a-RC6 中文汉化v1.0.0](https://www.fossic.org/thread-3060-1-1.html) 下载最新的汉化版游戏安装包。

### 下载 GitHub 上的最新汉化

如果您希望抢先体验汉化内容，请参照如下步骤下载汉化：

1. 下载汉化文件
   1. [点这里下载汉化文件](https://github.com/TruthOriginem/Starsector-0951-Localization/archive/refs/heads/main.zip)
   3. 解压下载的文件，其中应包括名为`localization`的文件夹
2. 安装汉化文件
   1. 打开游戏目录下的`starsector-core`文件夹
   2. 将下载解压文件中`localization`文件夹内的全部内容复制到`starsector-core`文件夹中
      1. 如提示文件已存在，请选择【覆盖】
3. 正常游玩，**如果遇到翻译质量问题或bug，请及时向我们报告**

## 参与汉化

如希望参与汉化，请加入远星汉化组，并使用Paratranz平台进行翻译：

1. 通过 QQ 553816216 添加 **议长** 的好友，或者申请加入QQ群 788249918 **汉化顾问团**，添加好友/申请入群时**请注明你的来历和英语水平**。
2. 参照[这个指南](docs/tut_translator.md)使用Paratranz平台进行翻译

## 译文格式规范

请参见[远行星号译文格式规范](docs/format_standard.md)

## 译名表

请参见[远行星号术语参考表](https://paratranz.cn/projects/3489/terms)

## 项目管理

### 文件夹结构

* "版本号 + data"是游戏各个版本原始的 data 文件夹
* "original" 内存放当前版本的英文原文，不要改动
* "localization" 内存放当前版本的译文
* "para_tranz" 内存放Paratranz平台相关脚本
* "docs" 内存放项目文档内容

### 自动化脚本

**Python环境: 3.8.5**

| 文件                  | 作用                                                    |
|-----------------------|-------------------------------------------------------|
| handleVariantNames.py | 处理指定文件夹中所有装配名，并更新/使用映射 json 用于翻译。                     |
| swapLangFile.py       | 用来更替汉化文件和英文文件的脚本。                                     |
| FindDifference.py     | 查找不同版本之间的差异。                                          |
| variant_name_map.json | 装配名映射文件，英文名对应汉化名，可后继继续更新。                             |
| para_tranz.py         | 用于ParaTranz平台的数据导入导出工具，使用方法参见[本指南](docs/tut_admin.md) |

### 版本汉化流程

![][flow-chart]

[flow-chart]:docs/flow_chart.png
