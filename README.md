Sass-Breakpoint
===============

如何使用Breakpoint来实现css媒体查询


1. 安装Sass 和 Compass (前提是安装过ruby)

(1). 安装Sass, 运行命令 sudo gem install sass
(2). 安装Compass, 运行命令 sudo gem install compass
(3). 安装Breakpiont，运行命令 sudo gem install breakpoint

2. 创建Compass项目,配置confi.rb文件

(1). 创建Compass项目,运行命令 compass create test
(2). cd /test, 在confi.rb 文件中添加 require 'breakpoint' 
(3). 在tes.scss 文件头部添加 @import "breakpoint"
(4). cd ../  运行命令 compass watch, 用来检测test文件夹中sass文件更改之后，自动生成css文件

3. 在sass文件中使用breakpoint来实现媒体查询

  @import "breakpoint";
  $basic: 543px;
  @include breakpoint($basic) {
    content: 'Basic Media Query';
  }
  
4. 按照sass里面的语法来书写你需要的代码


