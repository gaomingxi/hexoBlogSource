---
title: 如何将hexo博客源码托管GitHub
date: 2020-07-12 23:54:45
tags:
 - Hexo
---
> 如何将Hexo搭建的博客源码托管Git，方法也挺简单的，有几个有几个地方注意下即可
> * 创建一个新的github仓库并clon到本地
> * 将HEXO源码复制到刚才clon到本地文件夹
> * 上传github
> * **如何在另一台电脑上写作**

# 创建一个新的GitHub仓库+
相对比较简单的一个操作，直接在GitHub上操作即可，略过

# 复制代码
 将本地的源码，复制到刚才clone到本地的文件夹中；如果源文件中有.git文件，不要复制.git文件夹
 
 **源文件夹**
 ![源文件夹](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-13_00-08-19.png)
 
**执行清理命令**
```
hexo clean
```
![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-38-23.png)


**删除node_modules文件夹** 
![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-42-06.png)

**复制到新文件夹**
 ![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-13_00-13-55.png)

# 上传github
  已经完成源文件的迁移，下面将文件文件提交GitHub
 ![push](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-13_00-17-02.png)

 ![GitHub](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-13_00-19-33.png)

# 如何在另一台电脑上写作

 #### 切换到新电脑后，需要将源码clone到本地
 * 获取clone地址
 ![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-15_23-56-28.png)

 * clone到本地

 ![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-15_23-59-41.png)

* clone完成

 ![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-02-50.png)

 #### 在编辑器中打开项目
* 打开项目后，执行编译命令会报错，这个时候需要执行几个命令
![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-07-27.png)

 #### 需要执行几个命令
* 第一个命令
```
npm install hexo
```
![npm install hexo](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-09-35.png)

* 第二个命令
```
hexo init
```
![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-44-58.png)

如果遇到报错可忽略

* 第三个命令
```
npm install
```
![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-46-06.png)

#### 执行hexo命令

* 编译

```
hexo g
```
执行编译命令后没有报错、警告，则编码成功

* 启动
```
hexo s
```
![](https://picgo-blog.oss-cn-beijing.aliyuncs.com/img/hexo/Snipaste_2020-07-16_00-50-59.png)
