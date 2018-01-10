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



