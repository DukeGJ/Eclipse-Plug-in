Eclipse 具有丰富的菜单功能，给开发人员提供了很好的用户体验。总体而言，Eclipse 菜单种类包括视图 / 编辑器菜单，主菜单（Main Menu），视图 / 编辑器菜单（ViewPart/EditorPart Menu）和上下文菜单（Context Menu）。插件开发人员通过灵活应用这些菜单，可以给用户提供很好的体验。

**菜单项的扩展点**

Eclipse 提供了两种扩展点供用户添加菜单项到相应的位置。这两种扩展点为 org.eclipse.ui.commands（本文简称为 Commands 方式）和 org.eclipse.ui.actionSets（本文简称为 Actions 方式）。Actions 方式为界面上不同区域的表现方式提供了相应的扩展点，并且没有分离其界面表现和内在实现。恰恰相反，Commands 方式通过三步有效的达到界面表现和内部实现的分离：首先，通过 org.eclipse.ui.commands 扩展点创建命令和类别（Category），并且可以把某些命令放在一个类别（Category）中；然后，通过 org.eclipse.ui.menus 指定命令出现在界面的哪个区域（视图菜单 / 主菜单 / 上下文菜单）；最后通过 org.eclipse.ui.handlers 指定命令的实现。因此，Eclipse 推荐新开发的插件使用 Commands 来创建您的界面菜单。当然，由于 Actions 在现有的插件中用得比较多，如果我们需要扩展或基于之前的插件开发，也需要对其进行了解。除此之外，针对上下文菜单，虽然 Commands 和 Actions 方式均可以创建上下文菜单，但是 Eclipse 还提供了另外一种创建上下文菜单的扩展点 org.eclipse.ui.popupMenus（本文简称为 popupMenus 方式），下文仅详细介绍commands扩展点，其他的可以参看。

