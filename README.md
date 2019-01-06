# waterfall-sinanews
## 新浪新闻瀑布流布局练习
[预览地址](https://gzygzy00.github.io/waterfall-sinanews/)
## 懒加载原理
把 img 标签里的 src 指向一张默认图片，然后自定义一个 data-src 存放真正的图片地址；
当载入页面和监听滚动条，把可视范围的图片 data-src 替换到 src 里，即显示加载后的图片。
## 瀑布流原理
设置图片定位 position: absolute;
设置一个 colCount 根据图片宽度和容器宽度计算每一行图片个数，即列数；
设置一个 colHeightArrey 空数组，监听加载图片，数组储存一行中每一列图片的高度总和，并选出最小的一项，将其放在高度最低的一列下。
## 实现原理
使用ajax获取数据，然后拼装摆放到页面上，注意数据的读取...
