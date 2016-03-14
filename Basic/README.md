# 模板 - Templates

iOS的界面设计模板包含一套矢量格式UIKit组件集合。它有一个标签栏，导航栏，表视图，以及更多。您可以使用它创建一套设计原型。
操作路径`File\New From Template\iOS UI Design`，你会看到以下内容：
![](http://cdn1.raywenderlich.com/wp-content/uploads/2015/11/SketchNewTemplate.png)

注意这个菜单里也可以选择Android的`Material Design`设计模板。
打开之后你会看到一个包含各种iOS的UI组件的巨大模板。你可以通过在画布上拖拽选择各个控件，你可以通过按住`Command`，并使用鼠标滚轮进行画布缩放。


# 画板 - Artboards

你可以在Sketch这个无限大的画布上绘制你想要的任何图形，如果你要展现多个App屏幕的内容，那就要通过`画板`这个东西。画板组织一个固定的画布图层。当你导出画板，所有的图层将会合并成一个单一的文件。这里可以把它看做成Xcode里一个Storyboard的控制器场景(ViewController Scenes)。

通过执行以下步骤来创建一个新的画板：
+ 拖动画布，移动到一个空白区域。
+ 从左上方第一个功能按钮`Insert`，单击选择`Artboard`。
+ 在出现的右窗格中，选择`iPhone6`尺寸。

>注意：你看到的这个教程的UI模板可能会低于你所使用的版本，某些UI控件或者元素的位置可能会有不同，但这并不影响本教程的学习。

![](http://cdn3.raywenderlich.com/wp-content/uploads/2015/10/artboard.png)

创建之后你应该能看到一个叫做`iPhone6`的空白画板。默认情况下，新创建的画板将把它周围自由浮动的元素也都包含进去。这样肯定就煞笔了，所以我们还是按照上面的步骤，把默认的模板滚到别的地方，中间留出空白区域用于创建我们所需要的画板。
只要你爽，画板你想添加多少都行。`Sketch`有`iPhone`，`Apple Watch`，甚至`iPad Pro`的尺寸。如果你点错或者不想使用这个画板，选择删除即可，不用想太多。

>注意：如果你想要任意大小的画板，你可以`Insert\Artboard`，随便选择一个画板，任意拖动大小即可，至于命名，在左边的文件组织列表栏里把画布所在的分组栏重命名即可。


# 复制，粘贴

现在，你已经有了一个画板，从UIKit模板中拖动这几个控件。一个`Navigation Bar`，`Tab Bar`和`Table View Cell`。
虽然你可以复制和粘贴`⌘C和⌘V`，但这很难预测粘贴后控件出现的位置。所以还是老实点，按住`Option`键拖动一个控件，在你想要粘贴的地方松开鼠标左键即可。
![](http://cdn2.raywenderlich.com/wp-content/uploads/2015/10/steal-from-template.gif)

>提示：如何使用快捷键`⌘D`重复前面的动作。使用`Option`拖拽粘贴与`⌘D`创建多个副本：
>+ 选择一个控件直接按住`Option`键拖拽`Cell`到合适位置。
>+ 接着使用快捷键`⌘D`创建剩下的`Cell`。

>如上图演示一样，你有没有吃精呢？


#基础形状 - Basic Shapes

首先，新开个文件或者在画布上找个空白的地方插入一个画板：`Insert\Artboard`
接着，我们来搞个图形玩玩，`Insert\Shape`选择一个可用的形状。
![](http://cdn2.raywenderlich.com/wp-content/uploads/2015/10/shape-options.png)

>实际上，我们可以使用快捷键来插入新的形状。使用`快捷键O`再按住鼠标左键拖拽即可插入一个椭圆，同样使用`快捷键R`可以插入一个矩形。下面，罗列出一些常用的图形插入快捷键：
>+ L：插入直线快捷键
>+ O：插入椭圆快捷键
>+ T：插入文本快捷键
>+ R：插入矩形快捷键

有了这些，你可以自己动手画个机器人玩玩（过程中你可能需要调整下字体来达到相同的效果）。
![](http://cdn1.raywenderlich.com/wp-content/uploads/2015/10/smiley-robot.gif)

>注意：在插入的时候你可以按住`Shift`来保证图形绘制成圆形和正方形。


# 制作图形 - Styling a Shape

基础的形状虽然好，但是基本上不能给人留下深刻的印象，所以我们可以使用窗口右侧的`Inspector`栏来编辑图形的一些基础属性，比如颜色，边框半径啥的。这个东西你可以理解为`Xcode`的`Attributes Inspector`工具栏。
![](http://cdn2.raywenderlich.com/wp-content/uploads/2015/10/style-options1.png)

下面罗列的选项你可以多试试，熟悉一下：
+ 位置/大小 - Position/Size：对于有的图形或者画布很难拖动调整，你就可以利用这个选项调整画布，点击`Size`选项中间的`小锁图标`可以锁定比例，在调整大小的时候就会按照你想要的比例等比例缩放。
+ 半径 - Radius：这个选项应该不用解释太多应该都懂，就是调增矩形边角弧度半径的的一个滑块。
+ 透明度 - Opacity：看名字也知道了，同上，不多解释，下面会有很多示例。
+ 填充 - Fills：使用颜色选择器来改变图层的填充色，也可以取消透明填充。
+ 边框 - Borders：设置边框粗细和边框颜色，也可以完全禁用它。

>小贴士：Sketch自带有色彩拾取器，快捷键是`Control-C`，这完全是一个内置拾取器，非常方便。
![](http://cdn2.raywenderlich.com/wp-content/uploads/2015/10/color-picker.png)

有了这些，你可以跟着下面的动态图做学习下药丸的制作：
+ 使用快捷键`R`创建一个矩形。
+ 通过调整矩形边角半径`Radius`到`100`让其看起来像药丸。

![](http://cdn5.raywenderlich.com/wp-content/uploads/2015/10/pill-shape.gif)

就如刚才说的一样，你可以自己试试其他的设置，提升一下熟练度。


# 图层列表 - Layer List

这个功能区`图层列表 - Layer List` 位于窗口的左边，它包含了图层列表所包含的所有图层文件。图层是重叠起来的，结构类似于`Storyboard`中的视图层次结构。
文件组织层逻辑，你可以把多个图层作为一个单元一起移动，你还可以使用导出把它到合并成一个单一的对象并导出成图片。在图层列表中，组的概念用文件夹图标表示。

下列是图层组管理常用的快捷键：
+ ⌘G：选择多个图层拉进一个组。使用`⌘-Shift-G`键取消组合。
+ ⌘R：重命名选定的项目。Sketch里`回车键`只能展开组，不能重命名哈。
+ ⌘-Option-Up/Down：快速移动在组内移动图层，可以理解为iOS开发中视图的层级`index`的移动。
+ ⌘-Shift-L：锁定图层，让其在画布中不能被选择，即便是在图层列表选择也不能编辑。这个功能将在下一节使用。

![](http://cdn3.raywenderlich.com/wp-content/uploads/2015/10/layer-list.gif)

>提示：使用这些功能能让我们很好的组织图层结构，就如一个有洁癖的开发需要好的工程目录组织一样，快速定位和爽心悦目是必须的，比如动态图利演示的`TableView`和`Tab Bar`一样。然后你可以使用`⌘-Option-Up`组合快捷键把图层移动到整个画板前沿，避免被其他图层挡住。这里我们尽量不要选择拖拽来排列，避免不小心拖到一个组到另一个组里去了（老版本的`Xcode`经常有这鸟问题，一不小心组就拖错了）。

试试加些分组到你的`iPhone`画板里，记得多练习下分组命名。