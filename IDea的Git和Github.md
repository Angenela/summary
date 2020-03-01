---

---

# Git基础知识

- git的工作区：在当前仓库中，新增，更改，删除文件这些动作，都发生在工作区里面。
- git的暂存区：英文叫stage, 或index。在版本库.git）目录下，有一个index文件。它实际上就是一个包含文件索引的目录树，像是一个虚拟的工作区。在这个虚拟工作区的目录树中，记录了文件名、文件的状态信息（时间戳、文件长度等），文件的内容并不存储其中，而是保存在Git对象库（.git/objects）中，文件索引建立了文件和对象库中对象实体之间的对应。如果当前仓库，有文件更新，并且使用git add 命令，那么这些更新就会出现在暂存区中。

- 版本库：当前仓库下，如果没有任何的提交，那么版本库就是对应上次提交后的内容。 



# 在IDea中配置Git环境

![image-20200301130048013](C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301130048013.png)



# 创建本地库

![image-20200301125854608](C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301125854608.png)



# 选中需要创建的文件

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301130311090.png" alt="image-20200301130311090" style="zoom:50%;" />



然后在项目中会出现Git图标

![image-20200301130429829](C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301130429829.png)

且在项目目录中会有一个隐藏的.git文件

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301130542868.png" alt="image-20200301130542868" style="zoom:50%;" />



# Add和Commit

被标红的文件是工作区的文件，需要Add到暂存区

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301130915258.png" alt="image-20200301130915258" style="zoom:50%;" />

也可以Add整个项目



绿色的是在暂存区的文件，需要Commit到本地库

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301131240942.png" alt="image-20200301131240942" style="zoom:50%;" />

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301131709238.png" alt="image-20200301131709238" style="zoom:50%;" />



# 本地库Push到远程库

## 创建Github远程仓库

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301132727515.png" alt="image-20200301132727515" style="zoom:50%;" />



## 在Idea登录Github账号

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301132927765.png" alt="image-20200301132927765" style="zoom:50%;" />



## 配置远程端

![image-20200301133339371](C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301133339371.png)

将github远程仓库的地址配置到idea中

![image-20200301133510586](C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301133510586.png)

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301133527990.png" alt="image-20200301133527990" style="zoom:50%;" />



## 将项目Push到远程仓库

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301133243611.png" alt="image-20200301133243611" style="zoom:33%;" />



## Push成功后查看

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301133757229.png" alt="image-20200301133757229" style="zoom:50%;" />



# 克隆远程仓库

1. 可以在Github下载ZIP

2. 复制路径到IDea中操作

   <img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301134126847.png" alt="image-20200301134126847" style="zoom:33%;" />

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301134210442.png" alt="image-20200301134210442" style="zoom: 33%;" />



# 邀请朋友一起开发

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301134626611.png" alt="image-20200301134626611" style="zoom:50%;" />

这样别人Push的代码会更新到远程仓库上



# Pull

<img src="C:\Users\安基尼拉\AppData\Roaming\Typora\typora-user-images\image-20200301134916748.png" alt="image-20200301134916748" style="zoom:50%;" />

将远程仓库更新的代码下载到本地仓库



# 注意的问题

在Push时应该先Pull下来，以防版本冲突