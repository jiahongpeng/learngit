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










