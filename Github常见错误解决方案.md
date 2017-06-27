## 输入$ Git remote add origin git@github.com:xx/xxx.git错误
提醒错误：*fatal:remote origin already exists.*
解决方案：
> 1. 输入 **$ git remote rm origin**
> 2. 再输入 **$ Git remote add origin git@github.com:xx/xxx.git** 就没错误了
> 3. 若再出错， *error: Could not remove config section 'remote.origin'.*
> 4. 找到Github的安装路径，eg. **C:\Users\ASUS\AppData\Local\GitHub\PortableGit_ca477551eeb4aea0e4ae9fcd3358bd96720bb5c8\etc**
> 5. 找到一个名为gitconfig的文件，打开它把里面的 *[remote "origin"]* 那一行删掉就好了！


