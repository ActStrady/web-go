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

  - 块级元素
    1. 清除浮动 clear 一般使用both
    2. 背景图片平铺模式 background-repeat 取值：no-repeat、repeat-x、repeat-y repeat
    3. 背景图片位置 background-position 数值、top、left、right、bottom、center 也可以自定义值，注意负值的含义
    4. 列表样式 list-style-type 支持使用图片当列表 取值：none、disc、circle、square、decimal、upper-alpha、lower-alpha、upper-roman、lower-roman
    5. 设置定位类型 position  取值：relative(相对)、absolute(绝对)、fixed(固定，类似悬浮条)、static、inherit
    6. 设置元素与其包含块的边距的距离 top、left、right、bottom
    7. 设置内容溢出的处理方式 overflow  取值：visible（默认让其溢出）、hidden（减掉）、scroll（滚动）、auto（自动）、inherit（与默认差不多）
    8. 设置元素的层叠顺序 z-index  取值：数值、auto  表示的是几个叠在一起时在上在下 负数表示下边

  - 表格

    1. 是否合并单元格边 border-collapse: collapse 和cellspacing="0"效果类似 就是说把框线合在一起
    2. 设置表格布局 table-layout: auto 默认auto会根据内容撑开 fixed表示固定
    3. 设置单元格和表格边的距离 border-spacing: 0px类似于cellpadding="" 后者是内容与单元格的距离
    4. 设置caption位置 caption-side: bottom 上和下
    5. 空行单元格是否显示边框 empty-cells: hide


