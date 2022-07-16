# 译者注

_Effective Debugging_ by [Michael Yan](https://github.com/yanqi27)，讲述了如何更有效率地调试大型程序（以C/C++为例）的方法和技能。书中例子不仅丰富而且都是从实际的工作经验提取，观点和方法有效且具有可行性。

涉及的话题有：

- 内存管理器数据结构
- C/C++对象布局
- 如何拓展调试器
- 优化后的程序怎么调试
- 进程镜像
- 等等


我自己读了以后，受益匪浅，于是萌生了翻译成中文的想法。经过Michael的同意，于是开始了断断续续地翻译，在这个过程中，学到了许多，也加深了理解。

本书都是我自己理解了以后的翻译，并对书中原来使用gdb脚本的程序/脚本，使用了最新的[core analyzer](https://github.com/yanqi27/core_analyzer)作了替换。因为core analyzer是Michael改造gdb将书中的点子都变成了gdb里面的命令，使用更方便以及更强大。

有些我自己的理解，标记开头为XT，如，

XT: 举个例子可能会更好理解，如果申请32字节，那么返回的内存块的地址必须是可以整除32

限于本人水平，错误难免，请大家不吝赐教，或者提PR.

## 关于作者

http://core-analyzer.sourceforge.net/index_files/Page525.html

## 关于译者

https://www.zhihu.com/people/lan-tian-89

## 一些说明

- 有一些因为暂时找不到跟英文对应比较的词语，要么保留英文词，如bug；要么我自己根据自己的理解选了词，如unwind callstack，回卷调用栈。如果有更好的翻译，请不吝赐教。

- 如果有一些内容我不理解，我在翻译的附近标上(??)，提示可能翻译错误。

- 可能会添加一些章节，因为现在新的调试技术的出现。

