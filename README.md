# element

##目标：
效果页 https://element.eleme.cn/#/zh-CN/component/tabs
##1. 完成tab切换demo
  - HTML/CSS/JS
    -div.container
      - div.header => Tabs标签页: span.tab-header
      - div.content => Tabs面板：div.tab-panel
  - CSS
    - div.container 设置最大宽度，margin居中,加浅浅的边框 //h4的margin很大给container加一个小些的padding 16px
    - tab-header 在效果页选中elements查看颜色，规划字体大小，padding等等
    - tab-panel
      - 给第0个tab-panel加一个active样式~
      <!-- - 提供::hover伪类样式 -->
  - JS
    - 给active元素绑定onclick事件
      - 遍历得到类数组对象 => 将类数组对象所有DOM节点进行删除类操作
      - 给自己添加类操作

##2. 实现tab之间切换时候蓝色线是滑过去的
增加line元素。
- 覆盖效果就是绝对定位。
  position: absolute
  - 需要注意的是.Line的父亲.header需要添加
  position: relative

##3. 将div.container封装为对象。
  - 使用语法糖class
    - 需要注意的是在书写构造函数constructor的时候
    不应为document.querySelector()，需要琢磨。
    应为$container.querySelector()

##4. 实现Collapse折叠面板
  - 利用面向对象这一核心思想：
  封装；和创建对象同步写，同样可以有面向过程的所见即所得效果。
  - 添加参数，可以有手风琴以及折叠面板的效果。
  - HTML要写的好，header以及panel要写在一个item里面，大幅简化代码。莫死板。
  - 在构造器中带多一个参数type，ne'w区分一下就阔以
