#Impala-3.2.0
Impala-3.2.0在CentOS7.6 aarch64移植过程中，涉及的impala、kudu、native-toolchain、hadoop-lzo的patch文件，生成rpm包的脚本文件

##涉及patch文件
1、apache社区impala 3.2.0基础上：impala-3.2.0-python-manually-install-aarch64.patch
2、cloudera社区kudu cdh6.3.2基础上：kudu-cdh6.3.2_gcc4.8.5_aarch64.patch
3、cloudera社区native-toolchain cdh6.x基础上：native-toolchain-aarch64-support-forcentos7.6-oncdh6.x.patch
4、cloudera社区hadoop-lzo master分支（commit-id：db2a8fa68f5f700c98da3f102e3d7d676571e9ff）基础上：hadoop-lzo-aarch64-for-centos7.6.patch

##涉及脚本文件
在制作rpm包--自动生成rpm包章节，需要自动生成impala、kudu、hive、bigtop-utils的rpm包，以下脚本提供一键生成功能
1、make-rpm-bigtop-utils-0.7.sh
2、make-rpm-hive-cdh6.3.2.sh
3、make-rpm-impala-v3.2.sh
4、make-rpm-kudu-cdh6.3.2.sh
