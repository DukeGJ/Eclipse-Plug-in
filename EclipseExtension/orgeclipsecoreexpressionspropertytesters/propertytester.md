id：唯一标识符

types：作用暂不明

namespace：命名空间

properties：属性（多个属性可以用逗号隔开）

class：必须扩展PropertyTester类，test\(\)方法必须实现

xml配置：

```
<extension
         point="org.eclipse.core.expressions.propertyTesters">
      <propertyTester
            class="com.test.PropertyTester"
            id="com.test.propertyTester"
            namespace="com.test.propertyTester"
            properties="com.test.propertyTester"
            type="com.test.PropertyTester">
      </propertyTester>
</extension>
```



