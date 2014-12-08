# 前端css规范
## 浏览器支持标准
| 浏览器 | 标准 |
| ------------ | ------------- |
| IE9-11 |  |
| IE8 |  |
| IE6-7|
|Chrome| A |
|Firefox| A |
|Safari| A |
|Opera| C |

C、D级须有用户升级提示

* A级 - 交互和视觉完全符合设计的要求
* B级 - 视觉上允许有所差异，但不破坏页面的整体效果
* C级 - 可忽略设计上的细节，但不妨碍使用
* D级 - 不可使用，提示升级

## CSS模块化组织
为更好组织与维护页面样式，引入SCSS预处理器及Compass库。开发中，应按功能分解大文件，实现模块化的文件组织

* 使用和完善现有SCSS库
* 单个CSS文件避免过大
* CSS文件嵌套不要超过一层，避免编译后文件体积过大

## 重用现有SCSS样式库
* 全局核心样式库 /assets/lib/
	
	浏览器重置、排版、布局、元素基础样式包括：
	
	* reset - 页面重置
	* variables - 通用变量
	* mixins - 通用mix函数
	* grid - 布局
	* form - 表单
	* button - 按钮
	
* 通用模块样式库 /assets/mod/

	为求UI、VI风格统一，站点需要的通用模块，如头、尾等等

	* header - 头
	* footer - 尾
	* nav - 导航
	* quick-login - 快速登录
	
	
* JS组件相关样式库 /assets/ui/

	js组件相关联的样式库

	* modal - 模态框
	* tooltip - 提示
	* carousel - 轮播
	* loading - 加载
	

**不要轻易改动样式库，改动后要经过全面测试**

## 文件规范
* 文件名必须由小写字母、数字、中划线组成 
* 文件必须用UTF-8编码，使用UTF-8（非BOM），在HTML中指定UTF-8编码，在CSS中则不需要特别指定因为默认就是UTF-8。 

## 代码规范
不强制约束代码风格，开发过程中使用CSSFormat和CSSComb工具自动化排版即可

性能优化

* 禁止在css中使用*选择符。 
* 如果没有边框时，不要写成border:0，应该写成border:none 。 
* background、font等可以缩写的属性，尽量使用缩写形式 。

## 注释规范

## 命名规范
使用有意义的或通用的ID和class命名：ID和class的命名应反映该元素的功能或使用通用名称，而不要用抽象的晦涩的命名。反映元素的使用目的是首选；使用通用名称代表该元素不表特定意义，与其同级元素无异，通常是用于辅助命名；使用功能性或通用的名称可以更适用于文档或模版变化的情况。 

命名时需要注意的点： 

* 规则命名中，一律采用小写加中划线的方式，不允许使用大写字母或 _ 
* 命名避免使用中文拼音，应该采用更简明有语义的英文单词进行组合 
* 命名注意缩写，但是不能盲目缩写，具体请参见常用的CSS命名规则 
* 不允许通过1、2、3等序号进行命名 
* 避免class与id重名 
* id用于标识模块或页面的某一个父容器区域，名称必须唯一，不要随意新建id 
* class用于标识某一个类型的对象，命名必须言简意赅。 
* 尽可能提高代码模块的复用，样式尽量用组合的方式 
* 规则名称中不应该包含颜色（red/blue）、定位（left/right）等与具体显示效果相关的信息。应该用意义命名，而不是样式显示结果命名。

### 推荐命名

1. 页面结构
	* 容器: container
	* 页头：header
	* 内容：content/container
	* 页面主体：main
	* 页尾：footer
	* 导航：nav
	* 侧栏：sidebar
	* 栏目：column
	* 页面外围控制整体布局宽度：wrapper
	* 左右中：left right center
2. 导航
    * 导航：nav
    * 主导航：mainbav
    * 子导航：subnav
    * 顶导航：topnav
    * 边导航：sidebar
    * 左导航：leftsidebar
    * 右导航：rightsidebar
    * 菜单：menu
    * 子菜单：submenu
    * 标题: title
    * 摘要: summary
3. 功能
    * 标志：logo
    * 广告：banner
    * 登陆：login
    * 登录条：loginbar
    * 注册：regsiter
    * 搜索：search
    * 功能区：shop
    * 标题：title
    * 加入：joinus
    * 状态：status
    * 按钮：btn
    * 滚动：scroll
    * 标签页：tab
    * 文章列表：list
    * 提示信息：msg
    * 当前的: current
    * 小技巧：tips
    * 图标: icon
    * 注释：note
    * 指南：guild
    * 服务：service
    * 热点：hot
    * 新闻：news
    * 下载：download
    * 投票：vote
    * 合作伙伴：partner
    * 友情链接：link
    * 版权：copyright



	

