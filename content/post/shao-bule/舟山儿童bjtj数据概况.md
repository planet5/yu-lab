---
title: "舟山儿童保健体检数据概况"
date: 2019-03-27
lastmod: 2019-03-28
draft: false
#slug: "zs-eb-bjtj"
keywords: [舟山, 保健体检]
tags: [舟山, 保健体检]
categories: [邵布勒]
author: "邵布勒"
---

# 舟山儿童保健体检数据概况

## 新老数据基本情况

- 老的数据（2015前）有**334179**条记录
- 新的数据（2015后）有**225385**条记录

新老数据合并后总共**559564**条记录

**图1. 儿童保健体检数据变量缺失情况（n=559564）**

![bjtj_missing_var](舟山儿童bjtj数据概况.assets/bjtj_missing_var.png)

将体检数据与fbeb(妇保儿保连接数据)合并后，能合并上djbh的数据有338795条，变量缺失情况如下：

**图2. 体检数据合并djbh后变量缺失情况（n=338795）**

![djbh_bjtj_missing_var](舟山儿童bjtj数据概况.assets/djbh_bjtj_missing_var.png)

## 合并DJBH后再合并专项档案

新老专项档案合并后有87213条记录，剔除重复记录后**84928**条。

体检数据：

1. 根据zxdaid剔除完全重复记录（就目前提取的变量）**1026**条
2. 再根据zxdaid与随访日期剔重完全重复**24**条
3. 最后根据zxdaid跟随访日期简单剔重18064条，剩下**319681**条。

bjtj合并上zxda后计算随访日龄，根据日龄定义随访的月龄:arrow_down::arrow_down::arrow_down:

**图3. 随访年份分布（限定在2000-2018年）**

![sf_year](舟山儿童bjtj数据概况.assets/sf_year.png)

**图4. 随访月份分布**

![sf_month](舟山儿童bjtj数据概况.assets/sf_month.png)

**图5. 随访儿童月龄分布（剔除异常值后）**

![sf_age](舟山儿童bjtj数据概况.assets/sf_age.png)

**图6. 根据随访日龄定义随访月份**

![sf_age_def](舟山儿童bjtj数据概况.assets/sf_age_def.png)

### 表1. 儿童随访月龄定义方法

| 日龄范围       | 定义月龄 | 日龄波动范围（天） |
| -------------- | -------- | ------------------ |
| 80≤日龄≤100    | 3        | 20                 |
| 170≤日龄≤190   | 6        | 20                 |
| 230≤日龄≤250   | 8        | 20                 |
| 260≤日龄≤280   | 9        | 20                 |
| 350≤日龄≤380   | 12       | 30                 |
| 530≤日龄≤580   | 18       | 50                 |
| 720≤日龄≤770   | 24       | 50                 |
| 890≤日龄≤940   | 30       | 50                 |
| 1070≤日龄≤1130 | 36       | 60                 |

其中，有556人在定义的同一个月龄中有≥1次随访记录（目前处理：简单剔重）

### 表2. 儿童连续随访情况（根据是否有体重信息）（n=38789）

| 连续随访                     | n     | n(同时有出生体重) |
| ---------------------------- | ----- | ----------------- |
| 3-6-(8\|9)-12-18-24-(30\|36) | 17085 | **17006**         |
| 3-6-9-12-18-24-36            | 7711  | 7675              |
| 3-6-12-18-24-36              | 16589 | 16498             |

