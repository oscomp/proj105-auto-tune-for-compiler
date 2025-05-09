# proj105-auto-tune-for-compiler
编译自动调优工具

### 项目描述

场景描述：编译器选项直接影响性能，部分选项对精度有影响；选项参数对于选项效果有影响；Lib库的选择对于性能和精度都有影响；编译选项、参数、lib库数量多，依赖人工调优经验和应用特点，当前业界主流的调优工具，都只能进行编译选项和参数的调优，优化目标也仅限于性能。

项目内容：支持基本的编译选项调优，另外需要支持各种lib库的自动化选择，以及其他多种优化目标，包括性能、精度、code size。  

技术参考：

1)  [openEuler A-Tune](https://gitee.com/openeuler/A-Tune)；

2）[IBM MILEPOST GCC](https://en.wikipedia.org/wiki/MILEPOST_GCC)

参考资料：[ctuning](http://ctuning.org/wiki/index.php/CTools:MilepostGCC)，[reproduce-milepost-project](https://github.com/ctuning/reproduce-milepost-project)

环境限定：

1. 操作系统版本：openEuler 22.03 LTS
2. 编译器版本：openEuler GCC 10.3.0

openEuler 是华为主导，社区开源的一个Linux的发行版，所有开发者、合作伙伴、开源爱好者共同参与，围绕客户的场景进行创新，有更多新的想法产生，创建多样性计算场景最佳操作系统。在通讯，金融、安全等多个领域有着广泛的应用。

### 所属赛道

2025全国大学生操作系统比赛的“OS功能挑战”赛道

### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2025全国大学生操作系统比赛”的章程和技术方案要求

### 项目导师

吴峰光

- gitee [benniaobufeijiushiji](https://gitee.com/benniaobufeijiushiji)
- email linda7@huawei.com

### 难度

较大

### 特征

- 对编译原理，ARM架构有一定了解
- 熟悉C/C++，Python，Ruby语言

### License

[木兰宽松许可证, 第2版](http://license.coscl.org.cn/MulanPSL2)  

## 预期目标

1. 支持调优目标选择功能：支持性能、精度、code size优化目标的自动调优，单目标自动调优效果达到人工调优相比O2提升幅度的90%以上。并合理支持多目标组合。
2. 支持编译选项筛选功能：支持识别、替换编译选项，根据优化目标筛选恰当的编译选项。
3. 支持编译选项、参数调优功能：自动分析运行结果，迭代调整编译参数。
4. 支持lib库管理功能：支持lib库自动安装，并根据调优目标链接合适的lib库。
5. 支持配置文件初始化功能：设计合理的调优配置文件，并支持一键生成不同调优目标的初始配置文件，便于用户进行调优配置。
