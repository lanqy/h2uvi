# h2uvi
How to Use vi

## 跳转

跳到当前文档的第一行
```text
gg
```

跳到当前文档的最后一行
```text
G
```

跳到第 n 行
```
nj
```

## 撤销操作

- u 命令取消最近一次的操作，可以使用多次来恢复原有的操作
- U 取消所有操作
- Ctrl+R 可以恢复对使用 u 命令的操作

## 复制操作

- yy 命令复制当前整行的内容到vi缓冲区
- yw 复制当前光标所在位置到单词尾字符的内容到vi缓存区，相当于复制一个单词
- y$ 复制光标所在位置到行尾内容到缓存区
- y^ 复制光标所在位置到行首内容到缓存区
- #yy 例如：5yy 就是复制 5 行
- #yw 例如：2yw 就是复制两个单词
- m,ny 复制第m行到第n行之间的内容,例如：3,5y复制第三行到第五行内容到缓存区

将所有行从打开文件复制到剪贴板

```text
:%y+
```
## 打开和创建文件

当前打开的目录创建一个文件

```text
:e %:h/filename
:w
```

## 查找和替换

至上而下的查找

- / 要查找的字符窜，其中 / 代表从光标所在位置起开始查找，例如：/work

至下而上的查找

- ? 要查找的字符窜 例如：?work

用 new 替换当前行中第一个出现的 old
```text
:s/old/new/
```

用 new 替换当前行中所有出现的 old
```text
:s/old/new/g
```

用 new 替换从第 n 行到第 m 行中出现的 old
```text
:n,m s/old/new/g
```

用 new 替换整个文档中出现的 old
```text
:% s/old/new/g
```
## 删除

删除操作(命令模式使用)

- x 删除光标处的单个字符
- dd 删除光标所在行
- dw 删除当前字符到单词尾包括空格的所有字符
- #x 例如 3x 删除光标处向右的三个字符
- #dd 例如 3dd 从当前行开始向下删除三行文本

从当前位置删除到文件的开头

```text
Vggx
```

从文件的开头删除的末尾

```text
VGx
```

从第 10 行删除到 100 行

```text
:10,100d
```

删除所有包含 error 这个单词的行

```text
:g/error/d
```
删除所有不包含 error 这单词的行

```text
:g!/error/d
```

删除所有空行

```text
:g/^\s*$/d
```
让我们分解这个命令：

- g - 全局命令
- ^ - 行的开头
- \s* - 零个或多个空格字符
- $ - 行尾
- d - Ex 命令删除

光标将位于第一行中包含“pattern”的第一行
你打开文件。

```text
:+/pattern
```

取消文件中搜索的高亮

```text
:noh
```

## 文件间切换

两文件间的切换
```text
Ctrl+6
```

下一个文件
```text
:bn      
```

上一个文件
```text
:bp      
```

列出打开的文件，带编号
```text
:ls       
```

切换至第n个文件
```text
:b1~n  
```
