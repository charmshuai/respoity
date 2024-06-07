GitHub

#关键字查询:
xx (python)awesome:查该标签下的xx(Python)项目
xx (python) tutorial:查询xx(python) 资料、书籍、文档
xx (socket)sample:查询对应技术(socket)的代码样本
#GitHub三要素:
##Repository 仓库:
仓库是github项目管理存储基本单位

一个仓库中存储一个项目，一个用户可以拥有多个仓库，一般仓库分为public，private
##Commit提交:
程序员在整个开发周期，有大量的对代码资源的选代和修改，都可以通过commit的方式进行记录,便于程序员回溯代码，即使这些代码被删除

提交便于使用者观察整个工程的开发流程以及设计流程
##Branch 分支:
在仓库中可以包含多个分支，分支才是代码文件的第一存储单位，默认的仓库主分支为master/main

不仅可以管理代码存储，便于多人协作开发

~~picture00000000000000000000000000000000000000000000000000000000000000000000~~
#仓库内容
Code，资源存储，代码资源，二进制，项目管理脚本，许可证等等

issues，使用时遇到的bug或进行提交，等待反馈

README，使用markdown语言编写，工程自述文件，开发进度，，版本更新，使用介绍等等

LICENSE 许可证:GPL2.0,3.0.Apahce 2.0，Mit，这些许可证，给使用者最大使用权限以及最少的限制

#Git软件，分布式版本控制系统
仓库管理软件，使用git管理私人代码或企业代码

  本地内容                           发布内容<br>
version 1.1(新版)\-\>Gt(更新)\-\>version 1.0(旧版)<br>
#设备认证
##1、让网站的账户与设备绑定，后续完成代码的管理，上传下载
```bash
	git init // 创建本地仓库 *后续对仓库的操作，都要在仓库位置(master)
```
```bash
	git config -list //查看git配置文件
```
###修改或添加config配置项
```bash
	git config --global user.name  //用户名
	git config --global user.email //注册邮箱
```
###生成本机密文
```bash
	ssh-keygen -t rsa -C“注册邮箱”	#创建本地密文 *去对应的目录下查找密文文件
```
rsa.pub 复制密文，粘贴到settings /-/>SSH key and GPG /-/> new ssh key /-/>粘贴

###测试关联是否完成
```bash
	ssh -T git@github.com	#ssh远程登录	
```
Markdown , 文本修饰语言 ， 用特殊符号修饰正文效果<br>

## 标题修饰符\#

# 标题修饰符(一级标题)
## (二级标题)
### (三级标题)
#### (四级标题)
##### (五级标题)

## 正文内容
   输出正文内容 , 但是如果需要换行,用\<br\> 标签

## 修饰正文
   *一段测试文本<br>*
   **一段测试文本<br>**
   ***一段测试文本<br>***
   ~~一段测试文本<br>~~
   这是一段测试文本， 将`关键字`，重点显示
## 分割线
   用\-\-\- 表示分割线

---

##引用效用\>表示
> 一级引用
>> 二级引用
>>> 三级引用
>>>> 四级引用

## 列表修饰符

### 无序列表\*
* 二次元游戏
  * 原神
    * 肖弓
* 大逃杀类
  * PUBG
  * APEX
### 有序列表 1.
1. 物理学
   1. 粒子物理
   2. 原子核物理
   3. 凝聚态物理
2. 计算机科学
   1. 分布式架构
   2. 云计
### 混合列表
1. 测试一级
   * 测试二级
   2. 测试

### 表格
名称|技能|排行
--|:--:|--:
蝙蝠侠|有钱|32
海王|游泳|16
闪电侠|跑|18

### 代码片段

```c
	#include <stdio.h>
	int main(void){
		printf("test code\n");
		return 0;

	}
```
```cpp
	#include <iostream>
```
```python
	#import <os>
```
```bash
	echo "ceshi"
	pwd
	ps aux
	ld -l
```
