1. 在github网上创建了一个repo, 然后在本地文件夹(E:\GitHub\pine)用vs2010创建了实际的工程。回到github上时，发现没有显示repo的文件。看说明貌似是要创建readme.md文件。创建readme.md后果然出现了repo的文件显示界面，但是只有readme.md，没有我的刚才在创建的代码文件，我想应该是没有提交代码。于是打开git shell，输入git push origin master,居然失败报错，说是由于我在远程的操作没有同步到本地化。于是输入git pull, 下载readme.md到本地，然后再输入git push origin master, 成功！
2. 记录一下此文件上传到github的过程：
   1) 在本地（E:\GitHub\pine）创建gitUsage.md, 编辑好内容。
   2) git shell里显示发生了变化, 提示符从E:\GitHub\pine [maste]> 变成了 E:\GitHub\pine [master +1 ~0 -0 !]>. 应该是检查到本地文件发生了变化.
   3) git shell里输入命令：
      git add gitUsage.md
      git commit (提示符[master]变成了绿色)
      git push (提示符[master]变成了亮蓝色)
