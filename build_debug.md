


## 未成功的尝试

在阅读 build/envsetup.sh 发现了 TARGET_BUILD_TYPE 选择的命令， 是 choosetype 。在运行
```shell
$ source build/envsetup.sh  #构建编译环境
```
后，就可以使用 choosetype 命令了，该命令运行结果：

```shell
Build type choices are:
     1. release
     2. debug

Which would you like? [1] 
```
选择 2 后，TARGET_BUILD_TYPE=debug 就被写入了编译文件中，接着运行命令  lunch ，该命令提供选择编译平台，

运行结果能展示当前编译的所有选项，能看到 TARGET_BUILD_TYPE=debug 。

但接着运行 make 后，也会有编译选项的输出，此时看到其中的 TARGET_BUILD_TYPE=release ，怀疑没配置成功。

最后，在 make 时手动增加选项如下：

```shell
$ make TARGET_BUILD_TYPE=debug
```