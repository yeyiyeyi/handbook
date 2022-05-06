# 本地代码与github远程的通信  
**第一步：下载git**   

根据自己的需求下载  
链接:<https://git-scm.com/downloads>   

**第二步：建立本地仓库**  

新建文件夹，使用`git init`  

**第三步：获取电脑公钥**  

*检查本地是否有公钥*  

`cd ~/.ssh`  
若是出现No such file or directory说明本机没有SSH密钥  

**创建密钥**  

ssh-keygen -t rsa -C "注册Github账户时用的邮箱"  
连续enter三次，创建完成,可以查看密钥的存储位置

找到`id_rsa.pub`复制下来  

**第四步：配置Github的SSH Key**  

进入Github 点击头像选择Settings,选择左侧菜单的SSH and GPG keys,然后点击右侧的New SSH key按钮，将复制的`id_rsa.pub`黏贴进Github的key文本框中，title随意  

**第五步：github新建项目**   

github右上角新建一个new repository  
然后复制他的SSH  

**第六步：关联本地仓库和Github仓库**  

在文件夹右键使用git push here 输入以下代码  
`$ git remote add origin [复制的SSH]`  

**第七步：推送本地到远程**  
***第一次推送：***  
`git push -u origin master`  
***之后推送***  
`git push origin master`  

