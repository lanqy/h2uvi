# h2uvi
How to Use vi


将所有行从打开文件复制到剪贴板

```text
:%y+
```
当前打开的目录创建一个文件

```text
:e %:h/filename
:w
```

## 查找替换


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
