# `ranger` - 终端下的文件管理工具

------

[`ranger`](https://ranger.github.io/) 是一个基于文本的文件管理器，以 `Python` 编写。    </br>

不同层级的目录分别在一个面板的三列中进行展示。     </br>

可通过快捷键， 书签， 鼠标以及历史命令在它们之间移动。     </br>

当选中文件或目录时， 会自动显示文件或目录的内容。    </br>

- 主要特性有:     </br>
  
  - [`vi`](https://wiki.archlinuxcn.org/wiki/Vi "Vi") 风格的快捷键，     </br>
  
  - 书签，     </br>
  
  - 选择，     </br>
  
  - 标签，     </br>
  
  - 选项卡，     </br>
  
  - 命令历史，     </br>
  
  - 创建符号链接的能力，     </br>
  
  - 多种终端模式，     </br>
  
  - 任务视图.     </br>

`ranger` 可定制命令和快捷键，包括绑定到外部脚本。    </br>

最接近的竞争者是 [`Vifm`](https://wiki.archlinuxcn.org/wzh/index.php?title=Vifm&action=edit&redlink=1 "Vifm（页面不存在）")， 有 `2` 个面板以及 `vi` 风格的快捷键，但是总体特性相对较少。    </br>

------

## 中文说明：

该仓库为本人正在使用的终端文件管理器（`ranger`）的配置文件。    </br>

- 主要修改如下：    </br>
  
  - [ ] 图片预览    </br>
  
  - [x] 代码高亮    </br>
  
  - [x] 压缩包预览    </br>
  
  - [x] 文件预览    </br>
  
  - [x] 启动栏绘制边框    </br>
  
  - [x] 显示行号    </br>
  
  - [x] 设置宽度比例为2：3：5    </br>
  
  - [x] 将`ranger`配色方案修改为`Dracula`    </br>

------

### 如何使用：

- ① 使用软件包管理工具安装`ranger`及其插件：    </br>
  
  ```shell
  # Debian and derivative distributions
  $ sudo apt install ranger w3m-img w3m libx11-dev libxext-dev ueberzug kitty ffmpegthumbnailer highlight atool
  # ArchLinux and derivative distributions
  $ sudo pacman -S ranger w3m ueberzug kitty ffmpegthumbnailer highlight atool libcaca lynx elinks
  # Install with HomeBrew
  $ brew install ranger libcaca highlight atool lynx w3m elinks poppler transmission mediainfo exiftool ffmpegthumbnailer
  # There are many others, so I won't list them all here.
  ……
  ```

- ② 克隆该仓库并将该仓库放置在`~/.config`文件夹下（或，直接将该仓库克隆至`~/.config`文件夹下）    </br>
  
  ```shell
  $ cp -rfpv ranger ~/.config
  ```

- ③ 经过如上两个步骤后，则可使用吾所配置的`ranger`终端文件管理器，请尽情享受吧~    </br>

> **注意：**    </br>
> 
> ① 若需自行配置，请使用`ranger --copy-config=all`命令将创建如下`4`个配置文件到`~/.config/ranger`文件夹内：    </br>
> 
> | 主要配置文件        | 作用                                     |
> |:-------------:|:--------------------------------------:|
> | `commands.py` | 包含以`Python`编写的各种函数的实现，用于修改`ranger's`行为 |
> | `rc.conf`     | 用于设置各种选项并将按键绑定到功能，就是设置快捷键              |
> | `rifle.conf`  | 决定使用哪个程序打开哪个文件                         |
> | `scope.sh`    | 一个`shell`脚本，用于生成各种文件类型的预览              |
> 
> ② 若需使配置生效，还需在默认`shell`的配置文件中添加如下内容：    </br>
> 
> ```shell
> export RANGER_LOAD_DEFAULT_RC=FALSE
> ```
> 
> 若使用的默认`shell`为`bash shell`，则配置文件为`~/.bashrc`；    </br>
> 
> 若使用的默认`shell`为`zsh`，则配置文件为`~/.zshrc`。    </br>

------

### 免责声明：

此为本人学习使用。      </br>

由此提供对您的网站或计算机造成严重后果的本站概不负责。      </br>

此为纯属个人学习使用，禁止任何机构及个人将此系统作为商业用途！      </br>

禁止修改并盗用他人名义在网上传播！      </br>

请在体验试用24小时之内删除销毁！      </br>

若同意以上条款，方可对此进行下载使用！      </br>

若已下载此中任何，即视为同意以上条款！      </br>

若有侵犯行为，请联系本人删除。    </br>

------

- 【本文参考】：[终端文件管理器(ranger)配置使用](https://www.bilibili.com/video/BV1ER4y1F72A)

------

## English Description：

The repository is a configuration file for the ranger (file manager under the terminal) that I am using.    </br>

[ranger](https://ranger.github.io/) is a text-based file manager written in [Python](https://wiki.archlinux.org/title/Python "Python").     </br>

Directories are displayed in one pane with three columns.     </br>

Moving between them is accomplished with keystrokes, bookmarks, the mouse or the command history.     </br>

File previews and directory contents show automatically for the current selection.     </br>

Features include: [vi](https://wiki.archlinux.org/title/Vi "Vi")-style key bindings, bookmarks, selections, tagging, tabs, command history, the ability to make symbolic links, several console modes, and a task view.     </br>

*ranger* has customizable commands and key bindings, including bindings to external scripts.     </br>

Ranger also comes with its own [file opener](https://wiki.archlinux.org/title/File_opener "File opener"), [rifle](https://man.archlinux.org/man/rifle.1).     </br>

The closest competitors are [Vifm](https://wiki.archlinux.org/title/Vifm "Vifm") and [lf](https://github.com/gokcehan/lf).    </br>

- The major changes are as follows：    </br>
  
  - [ ] preview picture    </br>
  
  - [x] Code highlighting    </br>
  
  - [x] Compressed package preview    </br>
  
  - [x] File preview    </br>
  
  - [x] Draw a border for the launch bar    </br>
  
  - [x] display line numbers    </br>
  
  - [x] Set the width ratio to 2：3：5    </br>
  
  - [x] Modify the color scheme `ranger` to `Dracula`    </br>

------

### How to use：

- ① Install ranger and its plugins using the package management tool：    </br>
  
  ```shell
  # Debian and derivative distributions
  $ sudo apt install ranger w3m-img w3m libx11-dev libxext-dev ueberzug kitty ffmpegthumbnailer highlight atool
  # ArchLinux and derivative distributions
  $ sudo pacman -S ranger w3m ueberzug kitty ffmpegthumbnailer highlight atool libcaca lynx elinks
  # Install with HomeBrew
  $ brew install ranger libcaca highlight atool lynx w3m elinks poppler transmission mediainfo exiftool ffmpegthumbnailer
  ……
  ```

- ② Clone the warehouse and place the warehouse in `~/.config` folder (or, directly clone the repository to the `~/.config` folder)    </br>
  
  ```shell
  $ cp -rfpv ranger ~/.config
  ```

- ③ After these two steps, you can use the Ranger terminal file manager that I have configured. Enjoy~    </br>

> **Note：**    </br>
> 
> ① To configure yourself, use the command `ranger-copy-config = all` to create the following 4 configuration files to `~/.config/Ranger` folder：    </br>
> 
> | The main configuration file | Effect                                                                                          |
> |:---------------------------:|:-----------------------------------------------------------------------------------------------:|
> | `commands.py`               | Contains implementations of various functions written in `Python` to modify `Ranger's` behavior |
> | `rc.conf`                   | Use to set options and bind keys to functionality, that is, to set shortcuts                    |
> | `rifle.conf`                | Decide which program to use to open which file                                                  |
> | `scope.sh`                  | A `shell` script that generates previews of various file types                                  |
> 
> ② To make the configuration effective, you need to add the following content to the default `shell` configuration file：    </br>
> 
> ```shell
> export RANGER_LOAD_DEFAULT_RC=FALSE
> ```
> 
> If the default `shell` is `shell`, the configuration file is `~/.bashrc`.     </br>
> If the default `shell` is `zsh`, the configuration file is `~/.zshrc`.    </br>

------

### Disclaimer：

This is for me to learn to use.     </br>

This site will not be responsible for any serious consequences to your website or computer.     </br>

This is for personal use only.     </br>

It is forbidden for any organization or individual to use this system for commercial purposes！     </br>

Forbid to modify and steal other peoples name to spread on the net！     </br>

Please delete and destroy it within 24 hours of experience！     </br>

If you agree to the above terms, you can download and use this！     </br>

If you have downloaded any of these, you are deemed to agree to the above terms！     </br>

If there is any violation, please contact me to delete.     </br>

------

- 【This article is for reference】：[Terminal file manager (Ranger) configuration](https://www.bilibili.com/video/BV1ER4y1F72A)
