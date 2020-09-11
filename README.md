# Emacs + Vim 高效写作环境 | 像写代码一样优雅的写作

![image-20200912070612549](https://tva1.sinaimg.cn/large/007S8ZIlly1ginhwr26uej30gn0bcqd0.jpg)

## Vim Mode Plus

###  工作模式

Vim Mode Plus 主要有两个模式，normal模式和 visual模式，其中normal模式下可以进行光标移动、删除复制粘贴等大部分操作；visual模式是自定义选中模式。

![image-20200911204545242](https://tva1.sinaimg.cn/large/007S8ZIlly1gimzz79twdj30jg0b2gmr.jpg)



###  进入和退出 NORMAL 模式

- 通过以下方式进入
- - Caps Lock 
  - Left-Control + i
- 通过以下方式退出:
  - i、a 
  - caps lock,
  - esc,
  - control+[,
  - 单击鼠标任意按钮
  

###  NORMAL 模式可用键位说明:

| 键位 | 功能         |
| ---- | ------------ |
| h    | 向左移动光标 |
| j    | 向下移动光标 |
|  k    |  向上移动光标	 |
|  l    |  向右移动光标 	 |
| e    | 将光标移动到下一个词尾                 |
| b    | 将光标移动到上一个词开头          |
| 0    | 将光标移动到行首（在任何选项卡之前）
| ^    | 将光标移动到行首（在任何标签之后） |
| $    | 将光标移到行尾                    |
| g,g  | 将光标移动到文档的开始               |
| G    | 将光标移到文档末尾                 |
| {    | 将光标移到段落的开头              |
| }    | 将光标移到段落末尾               |



* 注意：这些键位可与 shift，control，option和/或 command 配饰使用，例如 在 normal 模式下 Control + h/l 可以左右切换桌面。

**删除组合键：**

| 键位            | 功能                             |
| --------------- | -------------------------------- |
| d,d / y,y / c,c | 删除/复制/剪切整行               |
| d,e / y,e / c,e | 删除/复制/剪切到下一个词尾       |
| d,b / ... / ... | 删除/复制/剪切到单词的前一个开头 |
| ...             | 同上，适用于上述所有其他导航键   |

**左右删除:**

| 键位 | 功能     |
| ---- | -------- |
| x    | 向右删除 |
| X    | 向左删除 |

| 键位      | 功能         |
| --------- | ------------ |
| p or P    | 粘贴到光标处 |
| u         | 撤销         |
| control+r | 重做         |

### 在特定的位置退出正常模式:

| 键位 | 功能                               |
| ---- | ---------------------------------- |
| i    | 在光标处退出 NORMAL 模式           |
| I    | 在行的开头退出 NORMAL 模式         |
| A    | 在行尾退出 NORMAL 模式             |
| o    | 在光标下方的新行上退出 NORMAL 模式 |
| O    | 在光标上方的新行上退出 NORMAL 模式 |

### VISUAL 模式可用键位说明

  **在 NORMAL 模式下，您可以通过 v 切换到 VISUAL 模式**：

| 键位 | 功能                                 |
| ---- | ------------------------------------ |
| v    | 退出 VISUAL 模式，进入   NORMAL 模式 |
| h    | 向左选择                             |
| j    | 想下选择                             |
| ...  | 同上，适用于上述所有其他导航键 |
| d    | 删除 (“剪切”) 选择并进入 NORMAL 模式      |
| y    | 选中 (“复制”) 所选内容并进入 NORMAL 模式       |
| c    |  (“剪切”) 选择并完全退出 Vim 模式 |
| x    | 删除选择并进入 NORMAL 模式              |

## 使用我的配置

1. 下载并安装[karabiner-elements](https://karabiner-elements.pqrs.org/)
2. 备份默认配置

    ```
    sudo mv ~/.config/karabiner/ karabiner.bak
    ```
3. 下载此配置

    ```
    git clone https://github.com/zuorn/karabiner-config ~/.config/karabiner
    ```





