###git基础命令使用

说明：
1.xxxxx代表某个commit号

查看远端地址</br>
git remote -v

git log
查看本地log ，不包括git reset --hard xxxxx 之后的所有内容，因为之后的所有内容已经被去掉了，本地看不到了
此命令可以显示从此时到之前的所有log

git log xxxxx
查看从xxxxx开始往后的所有log


git reset --hard 906a011e9f857c1e2bb2d77a3b93c2fa88622363
恢复到某一处修改，本地的文件改变了，但是远端的文件没有改变


git reflog
查看所有的操作

git reflog 906a011e9f857c1e2bb2d77a3b93c2fa88622363
查看所有的本地操作，如果通过--hard误"删除"某个文件，可以通过此命令恢复到固定的版本。
如果想恢复到某一个点，可以通过reflog查询出来的一些操作对应的commit号，使用
git reset --hard xxxxxx来恢复





