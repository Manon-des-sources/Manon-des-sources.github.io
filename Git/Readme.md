1、本地删除了一个文件，但是使用git pull命令却不能将删除的文件从GitHub再次pull下来。  
恢复操作：  
假如被删除的文件为 /test/file1.md  
如果是刚删除的、运行git status命令后、git会提示刚删除了的文件的路径  

执行git reset HEAD /test/file1.md  
git提示 Unstaged changes after reset  

执行git checkout /test/file1.md  
file1.md即可被恢复  
