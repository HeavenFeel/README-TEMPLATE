# README-TEMPLATE
A good readme.md file integration by me  after see some excellent readme.


> **目录**  
>- Introduction
>- Update Log
>- Catalogue Structure
>- Getting Started
>   - Requirements
>   - Versioning
>   - Built With
>   - Recommended modules
>   - Configuration
>   - Installation
>- Running the tests
>   - end to end tests
>   - coding style tests
>- Deployment
>- Troubleshooting
>- FAQ
>- Maintainers/Authors
>- License
>- Acknowledgments



#  Introduction 

在这里写 本项目的目的和功能,介绍应包括一个指向项目页面和 `issue queue`的链接。如果项目是`sandbox`，这些链接应该在升级之前到沙箱。

```
INTRODUCTION
------------

Project Title

The Administration Menu module displays the entire administrative menu tree
(and most local tasks) in a drop-down menu, providing administrators one- or
two-click access to most pages.  Other modules may also add menu links to the
menu using hook_admin_menu_output_alter().

 * For a full description of the module, visit the project page:
   https://xx.com/project/admin_menu

 * To submit bug reports and feature suggestions, or to track changes:
   https://xx.com/project/issues/admin_menu
```



## Update Log

```
### v1.0.0

https 升级

###  v0.1.0

增加 xx 需求
```




## Catalogue Structure

罗列大体的项目目录结构（在根目录下运行 `tree -L n` 即可生成目录结构图，n 指层级深度）




## Getting Started

### Requirements

`The requirements section (required)`, 需要清楚描述该project核心之外的部分(modules, libraries, etc).   
列出所有的requirements, 包括间接依赖另一个模块, etc.   
这个想法是告诉用户什么是必需的，这样他们需要的所有东西都可以在安装模块时获得并包括进来。
If there are no requirements, write `"No special requirements"`.
```
REQUIREMENTS
------------

This module requires the following modules:

 * Views (https://xx.com/project/views)
 * Panels (https://xx.com/project/panels)
```

### Versioning

```
VERSIONING
-----------

We use Git for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags/).
```

### Built With

```
BUILT WITH
-----------

- [Spring MVC](https://projects.spring.io/spring-framework/) - The web framework used
- [Maven](https://maven.apache.org/) - Dependency Management
- [Vue.js](https://vuejs.org/v2/guide//) - a progressive framework for building user interfaces. 
```


### Recommended modules 推荐模块

此可选部分列出不强制依赖的模块，但可能会增强项目的实用性或用户体验。确保描述启用这些模块的好处。

```
RECOMMENDED MODULES
-------------------

 * Markdown filter (https://xx.com/project/markdown):
   When enabled, display of the project's README.md help will be rendered
   with markdown.
```


### Configuration 配置

即使需要很少的配置，`The configuration section (required)`也是必需的。  
使用本节列出有关此模块配置的特殊说明，包括但不限于权限。 

如果`module`很少或没有配置，您应该使用此空间来解释启用/禁用模块将对站点产生什么影响。

```
CONFIGURATION
-------------
 
 * Configure user permissions in Administration » People » Permissions:

   - Use the administration pages and help (System module)

     The top-level administration categories require this permission to be
     accessible. The administration menu will be empty unless this permission
     is granted.

   - Access administration menu

     Users in roles with the "Access administration menu" permission will see
     the administration menu at the top of each page.

   - Display Drupal links

     Users in roles with the "Display drupal links" permission will receive
     links to drupal.org issue queues for all enabled contributed modules. The
     issue queue links appear under the administration menu icon.

 * Customize the menu settings in Administration » Configuration and modules »
   Administration » Administration menu.

 * To prevent administrative menu items from appearing twice, you may hide the
   "Management" menu block.
```
or
```
CONFIGURATION
-------------

The module has no menu or modifiable settings. There is no configuration. When
enabled, the module will prevent the links from appearing. To get the links
back, disable the module and clear caches
```


### Installation 安装

`The installation section (required*)` ,应清楚描述如何安装模块. 如果安装模块的步骤遵循软件标准说明，请勿重复- 只需提供一个链接，并详细解释可能会遵从这些步骤。  

如果您的安装说明非常复杂，请考虑将此部分替换为独立的INSTALL.md文件。

* - required ，除非提供`INSTALL.md`

```
INSTALLATION
------------
 
 * Install as you would normally install a contributed Drupal module. Visit:
   https://drupal.org/documentation/install/modules-themes/modules-7
   for further information.

 * You may want to disable Toolbar module, since its output clashes with
   Administration Menu.
```
结束一个例子，从系统中获取一些数据或使用它来进行一些演示。



## Running the tests

说明如何运行这个系统的自动化测试。


### Break down into end to end tests 分解成端对端测试

Explain what these tests test and why

```
Give an example
```

### And coding style tests 编码风格测试

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system



## Troubleshooting & FAQ

这部分是可选的。如果存在，它们应该解决问题队列中经常询问的问题（这将节省您将来的时间）。  
概述人们遇到的常见问题解决方案（如果步骤很长可以使用链接，但是通常应该提供摘要，因为链接有时会过时）。

```
TROUBLESHOOTING
---------------

 * If the menu does not display, check the following:

   - Are the "Access administration menu" and "Use the administration pages
     and help" permissions enabled for the appropriate roles?

   - Does html.tpl.php of your theme output the $page_bottom variable?

FAQ
---

Q: I enabled "Aggregate and compress CSS files", but admin_menu.css is still
   there. Is this normal?

A: Yes, this is the intended behavior. the administration menu module only loads
   its stylesheet as needed (i.e., on page requests by logged-on, administrative
   users).
```



## Maintainers/Authors

此部分是可选的，应替换任何预先存在的独立`MAINTAINERS.txt`文件。

```
MAINTAINERS
-----------

Current maintainers:
 * [Daniel F. Kudwien](https://drupal.org/user/54136/)  -  sun
 * [Peter Wolanin](https://drupal.org/user/49851/) - pwolanin
 * [Stefan M. Kudwien](https://drupal.org/user/48898/)  - smk-ka
 * [Dave Reid](https://drupal.org/user/53892/) - Dave Reid

This project has been sponsored by:
 * UNLEASHED MIND
   Specialized in consulting and planning of Drupal powered sites, UNLEASHED
   MIND offers installation, development, theming, customization, and hosting
   to get you started. Visit https://www.unleashedmind.com for more information.
```
```
AUTHORS
-----------
* Billie Thompson - Initial work - [PurpleBooth](https://github.com/PurpleBooth/)

See also the list of [contributors](https://github.com/your/project/contributors/) who participated in this project.
```



## License

```
LICENSE
-----------

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/your/project/LICENSE.md/) file for details
```



## Acknowledgments 致谢

```
ACKNOWLEDGMENTS
-----------
* Hat tip to anyone who's code was used
* Inspiration
* etc
```



> 以下是`README.md`的首选格式的摘要：
>
>- 标题全部大写
>- 标题用 `= ==/--`，然后是换行
>- 标题前空两行(第一个除外) 
>- 由星号 (*)表示的子选项与悬挂缩进
>- 列表编号缩进4个空格
>- 项目符号列表缩进1个空格
>- 每行80个字符


