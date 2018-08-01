### 解决Permission denied (publickey).
先进入Git命令行下
输入：
```
ssh-keygen -t rsa
```
之后一直回车
<br>
会在C:/Users/{yourname}/.ssh文件夹中生成id_rsa,id_rsa.pub两个文件
<br>
带有pub的即公钥，另一个为私钥,如下图：
<br>
<br>
![](https://github.com/Bihanghang/Test/blob/master/MarkDownPictures/Capture.PNG)
<br>
<br>
接下来找到Github上的这个页面
<br>
<br>
![](https://raw.githubusercontent.com/Bihanghang/Test/master/MarkDownPictures/githubSSH.PNG)
<br>
<br>
重新创建一个SSH key，名字随便起，
将id_rsa.pub的内容复制过来就解决了问题啦
<br>
<br>

```
![rejected] master -> master (fetch first)
````
如果报这个错，说明远程仓库已经有修改了，
所以需要先把远程仓库的内容先抓过来，
```
pull -all
```
比较暴力一点就是无视掉：
```
git push -u origin master --force
```




