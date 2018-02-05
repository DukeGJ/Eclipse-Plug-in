**Button（按钮）**

常用的SWT组件

**Style（样式）**

| SWT.NONE | 默认按钮 | ![](/assets/none.png) |
| :---: | :---: | :---: |
| SWT.CHECK | 多选按钮 | ![](/assets/check.png) |
| SWT.PUSH | 普通按钮 | ![](/assets/push.png) |
| SWT.RADIO | 单选按钮 | ![](/assets/radio.png) |
| SWT.BORDER | 深陷型按钮 | ![](/assets/border.png) |

**使用方法**

```
//单一样式
Button button = new Button(parent, SWT.NONE)
//组合样式
Button button  = new Button(parent, SWT.CHECK | SWT.BORDER | SWT.LEFT);
```



