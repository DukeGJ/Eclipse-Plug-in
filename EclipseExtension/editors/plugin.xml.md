在扩展编辑器中新增扩展点，配置好的plugin.xml文件如下：

```
   <extension
         point="org.eclipse.ui.editors">
      <editor
            class="com.testrcp.myrcp.editors.JsEditor"
            contributorClass="com.testrcp.myrcp.editors.JsEditorContributor"
            default="false"
            icon="icons/alt_about.gif"
            id="com.testrcp.myrcp.editors.JsEditor"
            name="JsEditor">
      </editor>
   </extension>
```

扩展点元素说明：

* point：编辑器的扩展点类型为org.eclipse.ui.editors
* class：与视图一样，一个编辑器对应一个class类，该类必须实现了org.eclipse.ui.IEditorPart类
* id：该编辑器对象的唯一标识
* name：编辑器显示的名称
* default：是否要使用默认的编辑器
* icon：编辑器显示的图标
* contributorClass：实现了org.eclipse.ui.IEditorActionBarContributor接口的类，Eclipse中EditorActionBarContributor类已经实现了该接口，通常的做法是继承该类，然后覆盖父类中的方法实现的。

* extensions：打开该编辑器的所对应的文件的扩展名，例如“htm，html”。

* command：要运行以启动外部编辑器的命令。

* launcher：实现了org.eclipse.ui.IEditorLauncher的类。这样启动程序将打开外部编辑器。

* filenames：编辑器打开文件时可选的文件名。

* symbolicFontName：编辑器字体的名称。

* matchingStrategy：实现org.eclipse.ui.IEditorMatchingStrategy的类。这运行编辑器扩展提供一个策略，是编辑器的输入与指定的编辑器输入相匹配。

> class、command和launcher都是打开编辑器的方式，属性是互斥的。



