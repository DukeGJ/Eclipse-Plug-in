**Button（按钮）**

按钮包含普通按钮（SWT.PUSH）、单选按钮（SWT.RADIO）、多选按钮（SWT.CHECK）、箭头按钮（SWT.ARROW）、切换按钮（SWT.TOGGLE）五种类型；按钮可设置按钮的样式，文字对齐方式的样式有 SWT.LEFT、SWT.RIGHT 和 SWT.CENTER，设置按钮外观风格的样式有 SWT.FLAT 和 SWT.BORDER。

**Style（样式）**

| SWT.NONE | 默认按钮 | ![](/assets/none.png) |
| :---: | :---: | :---: |
| SWT.CHECK | 多选按钮 | ![](/assets/check.png) |
| SWT.PUSH | 普通按钮 | ![](/assets/push.png) |
| SWT.RADIO | 单选按钮 | ![](/assets/radio.png) |
| SWT.BORDER | 深陷型按钮 | ![](/assets/border.png) |
| SWT.LEFT | 按钮文字左对齐 |  |
| SWT.RIGHT | 按钮文字右对齐 |  |
| SWT.CENTER | 按钮文字居中 |  |

**使用方法**

```
//单一样式
Button button = new Button(parent, SWT.NONE)
//组合样式
Button button  = new Button(parent, SWT.CHECK | SWT.BORDER | SWT.LEFT);
```



