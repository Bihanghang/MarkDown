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
![](https://github.com/Bihanghang/Test/blob/master/MarkDownPictures/Capture.PNG)
<br>
接着打开Gitbub上面的SSH重新创建一个，名字随便起，用编辑器打开id_rsa.pub这个文件复制到新建的位置


