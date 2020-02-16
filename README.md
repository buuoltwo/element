# element

目标：
效果页 https://element.eleme.cn/#/zh-CN/component/tabs
1. 完成tab切换demo
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

2. 实现tab之间切换时候蓝色线是滑过去的
