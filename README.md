# Linux命令行使用教程

当大家在学习编程之前，基本都没有使用过命令行操作电脑。因为Windows和Mac非常易用方便，完全没有必要使用命令行。但是当开始学习编程，并计划把编程作为自己的职业后，不可避免的就会有越来越多的机会使用命令行。

电脑分为两类，一类是个人电脑，一类是服务器。个人电脑主要是Windows和Mac，这两个系统都实用图形界面操作。但是因为安全和稳定性的原因，服务器大部分使用的是Linux系统，程序员常常就要和服务器打交道，所以熟练Linux的基本命令行操作是非常必要的。

Linux系统下没有盘符的概念。只有 / 表示根目录。常用的命令的功能分为文件和文件夹的增删改查。以下是对应的英语和简写。

创建目录，make directory，mkdir
删除	，      remove	，           rm
移动 / 重命名，move，    	mv
复制，              copy，	       cp
罗列	，             list，        	ls


以下是实际操作中需要输入的命令。

1. 在当前目录下创建一个新目录newtask，输入命令：
mkdir newtask

2. 删除这个目录，输入：
rm -r newtask
因为删除的不是单个文件，而是一个目录，我们需要在命令后加一个 -r 表示递归的删除整个目录。如果要删除的是单个文件new.txt 可以直接输入命令： rm new.txt

3. 在当前目录下复制文件new.txt，输入命令：
cp new.txt new1.txt

4. 在当前目录下复制文件夹newtask，则也需要加入 -r ，命令是：
cp -r newtask newtask1

5. 当前目录下创建一个新文件new.txt，命令是：
touch new.txt

6. 重命名new.txt 为new3.txt，命令式：
touch new.txt new3.txt

7. 查看当前目录下的文件，命令是：
ls

    查看当前目录下所有的文件和目录：ls -a            
    a表示all，所有的。

    查看当前目录下所有的文件的和目录，用完整的信息显示：ls -al                    
    a表示all，所有的。l表示long，长的信息。

8. 显示当前目录，命令是：
pwd

9. 移动new.txt 到newtask文件夹：
mv new.txt ./newtask
此处命令中newtask前面的 . 表示当前目录，如果不加./ 文件将无法移到newtask文件夹中。

10. 把newtask中的new.txt移动到newtask1中：
mv ./newtask/new.txt ./newtask1    或者用绝对路径：
mv /c/users/clement/desktop/newtask/new.txt  /c/users/clement/desktop/newtask    (clement是当前电脑的用户名)

Linux命令行的使用看起来好难记，好麻烦，只要坚持使用和联系，自然就能孰能生巧。不用畏惧和没信心，和记单词一样的。