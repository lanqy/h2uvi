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
