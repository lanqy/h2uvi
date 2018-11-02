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
