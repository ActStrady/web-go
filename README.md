### Web学习与复习
- html部分
  - 通用的几个属性
    1. title 设置元素的文本标题，在鼠标指向时会悬浮出标题
    2. tabindex 指定元素在tab键遍历控件时的访问顺序，就是说按tab键时的访问顺序
    3. 表格属性 cellspacing 单元格间距 cellpadding单元格内边距
  - 几个常用标签
    - head 标签
      1. mate 提供关于页面的描述信息 比如设置字符集和用于搜索引擎的关键字
    - body 标签
      1. span 一般做为css的钩子来使用，就是给块级元素里的某内容添加不一样的样式，是行内样式。
      2. lable 为表单类创建一个有意义的标记，一般使用for属性来关联表单控件 与其**id**名一样
      3. img 图片 属性alt表示加载不出图片的提示
      4. ul 无序列表 子元素是li 比较常用
      5. ol 有序列表 type可以选择列表类型
      6. dl dt dd 好像不是很常用的列表
      7. table里有thead tbody caption tfoot 浏览器会默认帮我们加上tbody，所以注意编码规范
---
- css部分
  - css选择符及优先级
    1. 全体选择符 * {}
    2. 元素选择符 a {}
    3. 类（class）选择符 . {}
    4. id选择符 # {}
    5. 伪类选择符 ： {}
    6. 后代选择符 . h3 {}
    7. 组合选择符 . . {}
    8. 分组选择器 1, 2 {}
    优先级：7>....1 8单独算
---
  - 文本
    1. 首行缩进 text-indent 可以应用于任何块级元素 取值：0、数值、百分比

    2. 对齐方式 text-align 取值：left、center、right、justify（两端）

    3. 处理空白 white-space 取值：pre 保留空白 nowrap 文本不换行 normal 忽略空白 

       一般用在td里用nowrap属性

    4. 行高 line-height  取值：数值、%、normal 一般24px~25px是常用的值

    5. 设置文本的垂直对齐方式 vertical-align 取值：%、baseline、super、bottom、sub、top、text-top、text-bottom、middle 用在行级元素

    6. 设置文字间距 word-spacing  取值：数值、normal

       实际效果其实就是增大一段文本中空白字符（空格）的宽度（整段汉字可能会没有效果，因为汉语段落一般都没有空格）

    7. 设置字母间距 取值：数值、normal  实际效果：在每个字母或汉字中间插入一段空白距离

    8. 设置文本效果 text-decoration 取值：none、underline、overline、line-through、blink

    9. 字体名称 font-family

    10. 字体大小 font-size 一般都是直接赋值的方式，常用12px、14px大小

    11. 设置字体粗细 font-weight 取值：normal、bold、bolder、lighter、数值，数值很少使用
---
  - 块级元素
    1. 清除浮动 clear 一般使用both
    2. 背景图片平铺模式 background-repeat 取值：no-repeat、repeat-x、repeat-y repeat
    3. 背景图片位置 background-position 数值、top、left、right、bottom、center 也可以自定义值，注意负值的含义
    4. 列表样式 list-style-type 支持使用图片当列表 取值：none、disc、circle、square、decimal、upper-alpha、lower-alpha、upper-roman、lower-roman
    5. 设置定位类型 position  取值：relative(相对)、absolute(绝对)、fixed(固定，类似悬浮条)、static、inherit
    6. 设置元素与其包含块的边距的距离 top、left、right、bottom
    7. 设置内容溢出的处理方式 overflow  取值：visible（默认让其溢出）、hidden（减掉）、scroll（滚动）、auto（自动）、inherit（与默认差不多）
    8. 设置元素的层叠顺序 z-index  取值：数值、auto  表示的是几个叠在一起时在上在下 负数表示下边
---
  - 表格
    1. 是否合并单元格边 border-collapse: collapse 和cellspacing="0"效果类似 就是说把框线合在一起
    2. 设置表格布局 table-layout: auto 默认auto会根据内容撑开 fixed表示固定
    3. 设置单元格和表格边的距离 border-spacing: 0px类似于cellpadding="" 后者是内容与单元格的距离
    4. 设置caption位置 caption-side: bottom 上和下
    5. 空行单元格是否显示边框 empty-cells: hide
---
- js 部分
  1. 全局变量和局部变量，不使用var的都是全局变量，其他的和java一样
  2. 定义数组， new Array();  和[];
  3. js dom操作 createAttribute()创建属性节点  createElement()创建元素节点  createTextNode()创建文本节点
  4. NaN 是字符串转换成 数值时 报错了，就是一个NaN； 任何一个数值和NaN进行运算结果 是一个NaN; NaN不和任何一个值相等，包括自己
  5. window.onload 页面加载完成后 一般用于在head里写script时需要操作文档后面内容的时候使用
  6. nextSibling; 下一个节点 nodeType 节点类型
  7. 阻止默认事件的发生 event.preventDefault(); 比如跳转和表单提交
  8. focus() 聚焦到
  9. addEventListener(事件类型，函数) 动态添加事件
  10. event.target; 获取事件源
  11. parentNode 父节点
---
- jquery部分
  1. dom对象转成jQuery对象 ` $(dom)` ， jQuery对象转成dom对象 ` $(dom).get(0)` 通过get函数获取dom对象
  2. $(selector).each(function(index, element));  对 jQuery 对象进行迭代，为每个匹配元素执行函数。其中index代表位置，element表示当前的元素。
  3. $(selector).bind(event,data,function);  规定向被选元素添加的一个或多个事件处理程序 其中event代表事件，data代表参数，function代表执行的函数
  4. unbind(event, function); 参数可选event表示具体事件，function表示要解绑的具体函数
  5. hide 和 show 表示隐藏和显示
  6. next(), prev() 上一个同辈元素和下一个同辈元素 prevAll() nextAll() 上边所有的同辈元素和下边所有的同辈元素
  7. parent() 获得当前匹配元素集合中每个元素的父元素 parents() 获得当前匹配元素集合中每个元素的祖先元素children() 获得匹配元素集合中每个元素的所有子元素。
  8. text() - 设置或返回所选元素的文本内容   html() - 设置或返回所选元素的内容（包括 HTML 标记）  val() - 设置或返回表单字段的值   attr() 方法也用于设置/改变属性值。
  9. text(function(i,origText)   text()、html() 以及 val()  attr() 的回调函数, 参数的意义：第一个：被选元素列表中当前元素的下标，第二个是原始值。
  10. prop 方法     prop() 方法设置或返回被选元素的属性和值  prop() 方法应该用于检索属性值，例如 DOM 属性（如 selectedIndex, tagName, nodeName, nodeType, ownerDocument, defaultChecked, 和 defaultSelected），如需检索 HTML 属性，请使用 attr() 方法代替。
  11. find() 返回被选元素的后代元素
  12. filter(criteria,function(index)))  返回符合一定条件的元素 可选两个参数  criteria：选择器表达式、jQuery 对象、一个或多个元素， function(index) ：要执行的函数，结果是true就表示被选择，index表示集合中的位置，需要注意的是：this表示当前的dom元素。
---
- ajax部分
  1. 基本语法：$.ajax(*{name:value, name:value, ... }*) 里边的键值对代表属性
  2. 常用的属性有  url: 指定数据来源    type: 数据的请求类型    dataType: 返回的数据类型

  3. 常用的回调函数 success(*result,status,xhr*) 成功时 第一个参数是返回的结果   error(*xhr,status,error*) 不成功时 beforeSend(*xhr*)  请求前   complete(*xhr,status*) 完成后 失败和成功都会调用 TODO：关于参数的具体使用以后研究
