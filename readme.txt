$ mkdir learngit
$ cd learngit    //创建空目录
$ pwd//创建版本库的地址

$ git init//把这个目录变成可以管理的仓库

$ git add readme.txt //把文件添加到仓库

add只能add一个文件，commit能上传好多文件，所以可以add好多，然后再一次commit
$ git commit -m"wrote a readme file"  //文件提交到仓库

$ git status    //当前库的状态，有没有没有上传的文件    modified是变动的文件

$ git diff   //查看difference，有时候回车键之后会出现++++end，点击q退出记录

$ git all//显示对版本库的所有操作



$ commit的时候如果出现如图1的错误，则删除git文件夹里面的index.log文件


git add -A   // 添加所有改动

git add *     // 添加新建文件和修改，但是不包括删除

git add .    // 添加新建文件和修改，但是不包括删除

git add -u   // 添加修改和删除，但是不包括新建文件



在 commit 前撤销 add:

git reset <file> // 撤销提交单独文件

git reset        // unstage all due changes


add/commit 前撤销对文件的修改:

git checkout -- README.md  // 注意, add添加后(同commit提交后)就无法通过这种方式撤销修改



版本回退

head 表示当前版本，也就是最新的，上一个版本就是head^,上上个版本就是head^^, 
前100个版本就是head~100

$ git reset --hard HEAD^  //回退到上个版本     如果是add上，但是没有commit的话，可以用这个
所以你让HEAD指向哪个版本号，你就把当前版本定位在哪。

cd ../   //回到上一层

$ cat readme.txt   //查看文件内容

$ git reflog //记录每一次命令的commit id

$ git reset --hard commitid//指定回到某个版本


工作区和暂存区

在电脑能看到的目录，比如说learngit

版本库 

有一个隐藏的目录 .git,这个是版本库

版本库最重要的是称为stage 的暂存区，还有git 自动创建的第一个分支master，
以及指向master的一个指针叫HEAD，如图1

文件往git版本库添加的时候，分两步：

第一步：用git add 把文件添加进去，实际上就是把文件修改添加到缓存区；
第二步：用git commit 提交更改，实际上就是把缓存区的所有内容提交到当前分支。

git commit就是往master分支上提交更改。

需要提交的文件修改通通放到暂存区，然后一次性提交暂存区的所有修改


$ git diff HEAD -- readme.txt  //可以查看工作区和版本库里面最新版本的区别


$ rm test.txt  //删除文件管理器的文件

1.删除版本库中的文件
$ git rm test.txt   
$ git commit -m "fdfd"
2.删错了，因为版本库里还有呢，所以可以很轻松地把误删的文件恢复到最新版本：
$ git checkout -- test.txt
3.如果版本库没有了，想撤回，只能回退到上一个版本。
$ git reset --hard HEAD^


git checkout -- readme.txt意思就是，把readme.txt文件在工作区的修改全部撤销
命令中的 -- 很重要，没有--，就变成了“切换到另一个分支”的命令。













