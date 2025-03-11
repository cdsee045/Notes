[TOC]
### scoop
#### 添加软件源 Bucket
```
scoop bucket add extras ##添加官方软件源 extras 
scoop bucket add dorado https://github.com/h404bi/dorado  ##添加第三方 bucket源dorado
```

#### 安装与卸载软件
```
scoop search # 搜索 APP
scoop install <app>   # 安装 APP
scoop uninstall <app>  # 卸载 APP

scoop list  # 列出已安装的 APP
scoop status # 检查哪些软件有更新
```
***
<br>

#### 软件更新
```
scoop update # 更新 Scoop 自身

scoop update appName1 appName2 # 更新app1 app2

# 更新所有 app （可能需要在apps目录下操作）
scoop update *

# 禁止某程序更新
scoop hold <app>
# 允许某程序更新
scoop unhold <app>
```
***
<br>

#### 清除缓存与旧版本
```
scoop cache rm <app>  # 清除指定程序的下载缓存
scoop cache rm *      # 清除所有缓存
scoop cleanup <app>   # 删除某软件的旧版本
```