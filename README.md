# Collaborative-development

这是一个**教你如何进行<font class="text-color-1" color="#f44336">协同开发</font>的仓库**，你可以根据本仓库的简易教程学会如何快速拉取别人的项目进行协同开发。

我们先来从**逻辑**上理解一下协同开发：

我们在一个中央代码库中共享和管理代码的不同版本。开发者可以克隆项目、创建分支、提交更改，并将它们合并回主分支

基于上述的逻辑概念，其实我们可以用图片来表示协同开发：
![image](https://github.com/lishuangqiang/Collaborative-development/assets/142634204/9b852b37-9435-4043-af8d-b514f7ab17be)

现在我们就要按照上图的逻辑，**<font class="text-color-01" color="#f44336">完成一个协同开发任务</font>：**


----


 **尝试拉取我的这个仓库，把<font class="text-color-01" color="#f44336">你的姓名和github主页链接</font>尝试添加到README.md中，最终我会接收到你的pull request。我将把它合并到这个仓库的README.md中，因此最终我的仓库会出现你的名字和github链接主页**。



----

在正式尝试本次练习之前，我需要向你介绍<font class="text-color-01" color="#f44336">**两种方式**</font>完成这个任务：

### 第一种方式：github网页端完成

1. **fork我的仓库到你自己的仓库中。**
   ![2b3f11bf7f83e00622bd5331fd00b77](https://github.com/lishuangqiang/Collaborative-development/assets/142634204/9e43ceef-28d9-424c-b367-0c6389997725)

2. **在你自己的仓库中，对这个fork的仓库新建一个分支。**
   ![134d561320d069b8fd4a28e7d8a1aa8](https://github.com/lishuangqiang/Collaborative-development/assets/142634204/18fbbe0c-b72f-4ae8-b67a-6140a9bf1b4c)
   创建分支
   ![276580627e8e6c77ee81ba7e680c0d0](https://github.com/lishuangqiang/Collaborative-development/assets/142634204/99a7b0dc-fa8a-4642-a400-7e24b2adec5c)

 >   通常情况下，我们会为我们处理的每一个问题都创建一个分支，避免多任务开发下的混乱。


3. **在你创建的新分支下进行编辑，新增你的姓名和github主页**
   回到你自己fork的仓库下，切换分支到你刚才创建的分支。编辑README.md文件，尝试添加你的姓名和github链接
   ![添加姓名和github链接](https://markdown.liuchengtu.com/work/uploads/upload_ebe99e70db0eb2543c92fb6ae1731332.png)


> **<font class="text-color-01" color="#f44336">   请按照下图格式进行添加你的名称和github主页</font>**
   ![格式示例](https://markdown.liuchengtu.com/work/uploads/upload_45e3234e66653017475c2e93631e9c03.png)


4. **发起 pull request**
   当你添加完毕之后，在当前分支下点击上方的**Pull request**。点击绿色按钮创建一个新的**Pull request**。
   ![创建Pull request](https://markdown.liuchengtu.com/work/uploads/upload_96ad177843e2c47265b2da76df54cfcf.png)

   点击Pull requests 之后再次点击 **New pull request**
   ![New pull request](https://markdown.liuchengtu.com/work/uploads/upload_e926a66f93f7367d9984c3c1f8e00d28.png)

   因为我们是在demo分支中进行修改的，所以我们要将提交分支切换到这个demo分支，单击绿色按钮 ****Create pull request****，你就完成了一次修改提交
   ![完成提交](https://markdown.liuchengtu.com/work/uploads/upload_530842571f59077d870704167d17ee93.png)

当我看到你的申请之后，如果检查无误，我就会将你的修改合并到我的仓库中。这时你就可以在我的仓库中看到你添加的昵称和github链接
### 第二种方式：本地计算机完成
<font class="text-color-1" color="#f44336">这里需要用到git，因此如果你的电脑没有安装git，请先安装git。</font>


> 当你尝试使用本地计算机完成本次任务的时候，仍然需要先fork我的仓库到你自己的仓库列表中，这部分上面讲过，就不再赘述

1.**拉取这个项目到本地计算机中**

此时你有两种方式将项目拉取到本地

1. 使用git clone 获取这个项目
2. 在IDEA中从版本控制获取这个项目
![](https://markdown.liuchengtu.com/work/uploads/upload_d70cb1101d8496786c9914e860db4853.png)
在这个界面将自己刚才fork的仓库拉下来
![](https://markdown.liuchengtu.com/work/uploads/upload_db89e08054f7c6dec3205c01949d439b.png)

2.**新增上有仓库地址**

你需要在我的仓库中，获取我的HTTPS地址：
![](https://markdown.liuchengtu.com/work/uploads/upload_0079b9af18add1fc3dbddd2afc671bce.png)
之后在IDEA终端中执行下面这两条命令：

```bash
git remote add demo-cy https://github.com/lishuangqiang/Collaborative-development.git

git remote -v
```
在这里为了方便演示，我fork了一个别人的仓库，添加的上游地址也是别人的仓库。最终效果如图所示：

![](https://markdown.liuchengtu.com/work/uploads/upload_20f3c5de68e1d5f69fc59c8f2539d823.png)

3.**创建分支**
​ 1.首先创建一个分支

```bash
git branch newBranches

```

​ 2.切换分支，在demo2.0这个分支进行创作不会影响master分支

```bash
git checkout newBranches
```
4.**向README.md文件中新增你的昵称和github链接**
![](https://markdown.liuchengtu.com/work/uploads/upload_47296b9da6d7ce23970f11d48a50aa12.png)

5.**进行提交**
![](https://markdown.liuchengtu.com/work/uploads/upload_b4503f16172ba42fd21e58309d69d356.png)
![](https://markdown.liuchengtu.com/work/uploads/upload_3bfa864bb034eac4f97fbec85f4f8e48.png)
之后我们在我们github的这个仓库进入 Pull request 就可以看到提交记录：
![](https://markdown.liuchengtu.com/work/uploads/upload_36a4058455f26de3daaa1a4b7db5e008.png)
之后点击****Create pull request****，我们就完成了一次修改提交。

通过上述介绍，我提供了两种方式来供你完成本次练习。现在就开始吧！祝你能够顺利的走进开源的大门，和世界各地的开发者协同开发

# 姓名表：（注意昵称和链接之间需要有空格）
  - [lishuangqiang] (https://github.com/lishuangqiang)
  - [Zephyr] (https://github.com/Arther-liaopan)
  - [zh-ao-ss] (https://github.com/zh-ao-ss)









