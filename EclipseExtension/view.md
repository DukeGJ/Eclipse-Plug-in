**介绍**：视图作为RCP最重要的扩展点，是与用户交互最多的界面

**扩展点**：org.eclipse.ui.views

**配置文件**：在扩展点编辑器新增扩展点，plugin.xml文件如下

```
<extension
         point="org.eclipse.ui.views">
      <view
            name="View"
            class="com.hirain.analysis.product.View"
            id="com.hirain.analysis.product.view">
      </view>
</extension>
```

**扩展点元素说明**：

* point：扩展点的类型为`org.eclipse.ui.views`
* id：该view视图的唯一标识符
* name：视图的名称
* class：视图对应的class类，该类必须扩展了`org.eclipse.ui.part.ViewPart`类
* catagory：
* icon：视图的图标
* fastViewWidthRatio：
* allowMultiple：
* restoreable：
* inject：



