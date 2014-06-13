BlendUI
==========

关于BlendUI
===

BlendUI能让Webapp的体验和交互与Native媲美。

具体而言，里面包括了两项关键能力：

1. 多Webview控制能力。让一个Webapp拆到多个webview中运行，并能用Javascript来调度。搞定了业务无解的难题：页面过大导致卡顿，页面切换不流畅，
2. Native组件嵌入能力。能将Native控件嵌入Webview中，这样就能让页面中那些性能较差的部分用Native来实现，以最大化地提高体验和交互。

与此同时，开发者看到的是Web API，不仅能快速上手，更由于BlendUI为普通浏览器完成了降级和替代方案，一套代码能同时在BlendUI环境和浏览器中同时运行。


Hello World
===

## 下载Javascript包

## 编写html页面

## 打包

Tips：可以在测试时，将`index.html`重定向到线上地址来方便调试，不用每次都打包。

API文档
===

http://fedev.baidu.com/~berg/docs/

背景和目标
===

最后再简单说说BlendUI的背景和目标。

在webapp和Native app之间，有一条无法逾越的鸿沟：体验和性能的差距。轻应用是webapp的延伸，同样存在此问题。为弥补这条鸿沟，我们要有一套方案，能让开发者使用web API，做出体验和性能与原生应用差距不大的应用。

经过一番调研，我们发现几个重要的现实问题，这些问题导致了webapp和native app之间的体验差距。

webapp缺少淡入淡出动画、转场动画、滑动动画，或者因此引起的不流畅，以及某些组件的弹力体验与原生有差距等。
浮动元素的处理。顶部、右侧、底部的固定位置的元素可能会有抖动，或者弹出菜单无法点按页面其他位置关闭，点按不流畅等。
输入框的问题。包括输入法无法正常展开收起，框内部滚动问题。
本地缓存能力。包括已浏览的图片本地缓存，静态资源缓存出现脏数据等问题。
DOM变化后的渲染抖动。包括无限下拉时的渲染抖动，无刷新翻页的闪烁
此外，vision mobile的调研数据显示，开发者之所以不选用html5的前三大原因是：

性能问题：45.7%
硬件接口有限：37.3%
难以集成原生组件：29.2%
因此，轻组件的首要目标是：弥补轻应用的体验劣势，包括页面间、页面内的转场动画，浮动元素处理，一些对性能要求较高的组件原生化等。

我们将面对的用户主要是高级web开发者。因此，库需要有足够的扩展性和灵活性，同时API必须是web化的。
