# 命令摘要

以下列表包含本教程前八页中提供的基本命令以及偶尔的使用示例（显示在括号中）。 它们的显示顺序与教程中出现的顺序大致相同。 （所有以冒号开头的命令后跟ENTER。）

- vi 在命令行键入以打开同一目录中的一个或多个文件
（vi tomato.txt 在当前目录中打开一个名为 “tomato.txt” 的文件）
（vi parsley sage rosemary 打开当前目录中的三个文件 “parsley”，“sage”和“rosemary”）
- vi * 在命令行键入以打开当前目录中的每个文件
- :q 关闭（退出）未进行任何更改的文件
- :q! 退出而不保存任何更改
- :w 将当前文件写入（即保存）到磁盘
- :wq 将缓冲区内容写入磁盘（即保存更改）并退出
- ZZ 与 :wq 相同
- i 激活文本插入模式，在光标的当前位置下立即插入文本
- h 将光标向左移动一个字符
（2h 将光标向左移动两个字符）
- j 将光标向下移动一行
（3j 将光标向下移动三行）
- k 将光标向上移动一行
- l 将光标向右移动一个字符
- G 将光标移动到所需的行;如果没有修改整数，则将光标移动到文本的最后一行 （5G将光标移动到第五行）
- a 切换到插入模式并允许立即在光标右侧插入文本
- x 删除光标下的字符
（xxx 立即删除光标下的字符，然后删除右边的两个字符）
- X 删除光标左侧的单个字符
- D 将当前行上的文本从光标下的字符移到行尾
- dw 删除光标下方的字符以及同一个字中右侧的剩余字符
（2dw 删除光标下面的字符，右边的剩余字符在同一个单词和所有下一个单词中）
- dd 删除包含光标的整行，然后光标移动到下一行
（2dd 删除以当前行开头的两个连续行）
- cw 删除光标下的字符及其右侧的字符，并允许输入新字符来替换它们
（2cw 删除光标下的字符，并在同一个单词和下一个单词中右侧删除，然后允许输入替换字符）
- cc 擦除当前行并允许输入替换文本
（2cc 删除当前行和下一行，并允许为两行输入替换文本）
- cb 删除当前单词中光标左侧的字符，并允许输入替换字符
（3cb 删除当前单词中光标左侧的字符及其左侧的两个单词，然后允许输入替换文本）
- R 激活文本输入模式，允许光标下方和右侧的文本一次覆盖一个字符
- xp 转换两个相邻的字符
- deep 转换两个相邻的单词
- ddp 转换两个相邻的行
- ~ 更改光标下字符的大小写
- J 将当前行与下一行连接起来
- u 反转已更改缓冲区的最新命令的效果
- U 撤消当前访问期间对当前行所做的所有更改
- :s/ 在文本中搜索指定字符串的第一个实例
（:s/cucumber 在文本中搜索字符串 “cucumber” 的第一个实例）
- n 在文本中搜索指定字符串的下一个实例
- :s/ / / 替换指定字符串的第一个实例
（:s/cucumber/radish/ 用字符串 “radish” 替换字符串 “cucumber” 的第一个实例）
- :%s/ / / 替换指定字符串的每个实例
（:%s/cucumber/radish/ 用字符串 “radish” 替换字符串 “cucumber” 的每个实例）
- :r 将文本从另一个文件插入当前打开的文件中
（:r lettuce.txt 将文本从名为 “lettuce.txt” 的文件中插入当前打开的文件中）
- 将当前打开的文件中的文本附加到另一个文件中
（:w>> cabbage 将当前打开文件中的文本附加到名为 “cabbage” 的文件中）

下一章：[vi 克隆](clones.html)
