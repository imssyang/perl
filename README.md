
https://www.cnblogs.com/f-ck-need-u/p/9685581.html

# 默认配置
~/.cpan/CPAN/MyConfig.pm

# cpan
o conf urllist push https://mirrors.aliyun.com/CPAN/
o conf makepl_arg INSTALL_BASE=/opt/perl
o conf mbuild_arg "--install_base /opt/perl"
o conf auto_commit 1
o conf prerequisites_policy follow
o conf urllist
o conf commit

# 安装模块
install CPAN ExtUtils::MakeMaker Module::Build Bundle::CPAN

# cpan
-a：创建CPAN.pm的autobundle
-D module：查看模块的详细属性信息。
   例如是否安装，安装的版本号，最新的版本号，对应的模块路径，对应的源码包文件路径，谁维护的
-g module：下载最新版本的模块到当前目录
-i module：安装指定的模块
-j Config.pm：指定CPAN配置数据的文件
-J：以CPAN.pm相同的格式dump当前的配置文件
-O：列出过期的模块
-v：输出cpan脚本的版本号以及CPAN.pm的版本号

eg:
cpan -i File::Util::Manual

# 查看文档
perldoc File::Util::Manual




