## 更新日志

### 2.0.0-beta3

*2020-09-04*

#### 新特性

- Button
  - click 事件抛出event对象 (by [@yawuling](https://github.com/yawuling)） )

- DatetimePicker
  - 新增方法 `toggle`, 在区域选择模式下，tab标签切换时触发 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `display-format-tab-label`, 在区域选择模式下，自定义展示tab标签文案的格式化函数，返回一个字符串 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 修改范围选择 交互样式，将picker拆分为 tab形式 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除插槽 `range-separator` (by [@HXCStudio123](https://github.com/HXCStudio123) )

#### 优化

- MessageBox
  - 动画时间由300ms改为200ms，减少等待时间
- Grid
  - 支持动态渲染GridItem （by [@HXCStudio123](https://github.com/HXCStudio123) ）
  - 支持列项修改后内部GridItem重排 （by [@HXCStudio123](https://github.com/HXCStudio123) ）
  - GridItem 内容padding移除，兼容小屏幕展示四字标题 （by [@HXCStudio123](https://github.com/HXCStudio123) ）

#### Bug 修复

- Cell
  - 修复边框线样式calc计算无效问题 (by [@yawuling](https://github.com/yawuling)） )
- ColPicker
  - 修复按需引入缺少actionSheet样式问题 (by [@yawuling](https://github.com/yawuling)） )
- Picker
  - 修复columns数据延迟传入无法正常展示文本问题 (by [@yawuling](https://github.com/yawuling)） )
- PickerView
  - 修复columns延迟传入时无法自动选中第一项的问题；修复columns延迟传入时picker重置数据的记录 (by [@yawuling](https://github.com/yawuling)） )
- Popup
  - 修复按需引入popup和messageBox缺少modal样式问题 (by [@yawuling](https://github.com/yawuling)） )
- StatusTip
  - 去掉占位图的白色背景，将图片从base64改为图片链接以减少包大小 (by [@yawuling](https://github.com/yawuling)） )
- Button
  - 圆角按钮圆角还原度，修复2px偏差 (by [@yawuling](https://github.com/yawuling)） )
- DatetimePicker
  - 修复 `DatetimePicker` 当type为 'date' 时，区域选择禁用错误选项，无法修改选中问题。 (by [@HXCStudio123](https://github.com/HXCStudio123) )

### 2.0.0-beta2

*2020-08-21*

#### 新特性

- Button
  - 属性 `type` 默认值为 `primary` (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Card
  - 新增卡片组件 Card  (by [@awjing](https://github.com/awjing) )
- Checkbox
  - 新增属性 `max-width`, 支持设置文字部分最大宽度，设置最大宽度开启文字折叠 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- ColPicker
  - 展开弹出框事件名称由 `showPicker` 改为 `open`。（by [@yawuling](https://github.com/yawuling)）
  - 新增方法 `close`, 支持关闭弹出框 (by [@yawuling](https://github.com/yawuling)） )
- DatetimePicker
  - 新增属性 `loading-color`, 支持修改加载的颜色 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 展开弹出框事件名称由 `showPicker` 改为 `open`。（by [@yawuling](https://github.com/yawuling)）
  - 新增方法 `close`, 支持关闭弹出框 (by [@yawuling](https://github.com/yawuling)） )
- DatetimePickerView
  - 新增属性 `loading-color`, 支持修改加载的颜色 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Loading
  - 属性 `type` 新增类型 `circular-ring` loading 样式 (by [@HXCStudio123](https://github.com/HXCStudio123) ) )
- Picker
  - 新增属性 `loading-color`, 支持修改加载的颜色 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 展开弹出框事件名称由 `showPicker` 改为 `open`。（by [@yawuling](https://github.com/yawuling)）
  - 新增方法 `close`, 支持关闭弹出框 (by [@yawuling](https://github.com/yawuling)） )
- PickerView
  - 新增属性 `loading-color`, 支持修改加载的颜色 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Radio
  - 新增属性 `max-width`, 支持设置文字部分最大宽度，设置最大宽度开启文字折叠 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- selectPicker
  - 新增组件 selectPicker 。 (by [@HXCStudio123](https://github.com/HXCStudio123))

### 2.0.0-beta1

*2020-08-14*

#### 新特性

- ActionSheet
  - 新增属性 `panels` 自定义面板，支持一维数组和二维数组，panel数据结构支持设置显示的图片地址和标题内容 (by [@awjing](https://github.com/awjing) )
- Badge
  - 新增属性 `top` 为正时表示角标向下偏移对应的像素 (by [@awjing](https://github.com/awjing) )
  - 新增属性 `right` 为正时表示角标向左偏移对应的像素 (by [@awjing](https://github.com/awjing) )
- Cell
  - 新增属性 `required`, 支持表单属性设置必填项 (by [@yawuling](https://github.com/yawuling) ) )
  - 新增属性 `vertical`, 支持表单属性展示为上下结构 (by [@yawuling](https://github.com/yawuling) )
- CellGroup
  - 新增属性 `border`, 支持设置表单组是否展示边框线 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- CheckboxGroup
  - 新增属性 `cell`, 支持复选框组下的表单模式事件 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `size`，支持单选框尺寸更改（large） (by [@yawuling](https://github.com/yawuling) )
- ColPicker
  - 新增 ColPicker 多列选择组件 (by [@yawuling](https://github.com/yawuling) )
- DatetimePicker
  - 属性 `value` 添加 `Array` 格式，用来支持区域选择下的 上方picker选中值 及 下方picker选中值。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `columns-height`, 支持设置 picker 内部的单个 pickerView 高 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `required`, 支持表单属性设置必填项 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `item-height` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `visible-item-count` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增默认插槽，可更改默认唤起 picker 的形式（默认为cell）。(by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增插槽 `range-separator`，区域选择时，中间展示的分隔符插槽。(by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 将 pickerView 交互形式更改为滚筒交互。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- DatetimePickerView
  - 新增属性 `columns-height`, 支持设置 pickerView 高 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `column-formatter`, 支持自定义处理列项数组，接收 pickerView 实例、pickerView 源数组 originColumns、pickerView 每个属性的范围 ranges、当前 pickerView 的 value 作为入参，根据选中项和边界范围进行判断，通过 pickerView 实例暴露出来的 getPickerValue 获取对数据进行数组转换 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `item-height` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `visible-item-count` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 将 pickerView 交互形式更改为滚筒交互。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Grid
  - 新增属性 `bg-color`, 支持宫格设置背景颜色 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Input
  - 新增属性 `no-border`, 支持设置取消底部边框 (by [@yawuling](https://github.com/yawuling) )
  - 新增属性 `required`, 支持表单属性设置必填项 (by [@yawuling](https://github.com/yawuling) )
  - 新增事件 `click-prefix-icon`, 点击前置图标时触发 (by [@yawuling](https://github.com/yawuling) )
  - 新增事件 `click-suffix-icon`, 点击后置图标时触发 (by [@yawuling](https://github.com/yawuling) )
- Loading
  - 属性 `type` 新增类型 `circle-outline` loading 样式 (by [@HXCStudio123](https://github.com/HXCStudio123) ) )
- Navbar
  - 新增默认插槽，可更改标题处展示样式。(by [@HXCStudio123](https://github.com/HXCStudio123) )
- NoticeBar
  - 新增属性 `type`， 新增默认插槽，支持设置通知栏类型。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 属性 `left-icon` 更名为 `prefix`。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 插槽 `left-icon` 更名为 `prefix`。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 插槽 `right-icon` 更名为 `suffix`。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Picker
  - 新增属性 `columns-height`, 支持设置 pickerView 高 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `required`, 支持表单属性设置必填项 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `item-height` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `visible-item-count` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 将 pickerView 交互形式更改为滚筒交互。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增默认插槽，可更改默认唤起 picker 的形式（默认为cell）。(by [@HXCStudio123](https://github.com/HXCStudio123) )
- PickerView
  - 新增属性 `columns-height`, 支持设置 pickerView 高 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `item-height` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `visible-item-count` (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 将 pickerView 交互形式更改为滚筒交互。 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Progress
  - 新增属性 `status` 设置进度条状态，支持sucess和danger (by [@awjing](https://github.com/awjing) )
- Popover
  - 新增组件 `Popover` (by [@HXCStudio123](https://github.com/HXCStudio123) )
- RadioGroup
  - 新增属性 `cell`, 支持单选组下的表单模式事件 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `size`, 支持单选框尺寸更改（large） (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Status Tip
  - 属性 `type` 下的七种类型 对应缺省展示图片更改。 (by [@awjing](https://github.com/awjing))
- Tabs
  - 移除属性 `color` (by [@awjing](https://github.com/awjing) )
  - 移除属性 `inactive-color` (by [@awjing](https://github.com/awjing) )
  - 移除属性 `line-width` (by [@awjing](https://github.com/awjing) )
  - 移除属性 `line-height` (by [@awjing](https://github.com/awjing) )
- Tabbar（TabbarItem）
  - 新增属性 `active-icon` 选中图标的类名 (by [@awjing](https://github.com/awjing) )
  - 新增属性 `top` 为正时表示角标向下偏移对应的像素 (by [@awjing](https://github.com/awjing) )
  - 新增属性 `right` 为正时表示角标向左偏移对应的像素 (by [@awjing](https://github.com/awjing) )
- Tag
  - 移除属性 `size` (by [@awjing](https://github.com/awjing) )
  - 新增属性 `mark` 标记类型 (by [@awjing](https://github.com/awjing) )
  - 新增属性 `round` 圆角类型 (by [@awjing](https://github.com/awjing) )
- Toast
  - 新增属性 `iconSize`， 支持修改左侧图标尺寸 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增属性 `loadingColor` ，支持设置加载指示器颜色 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 新增方法 `info` ，支持展示常规Toast样式 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Tooltip
  - 新增属性 `show-close`， 支持设置显示 Tooltip 内部右侧的关闭按钮 (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `effect` ，文字提示 2.0 起 不再支持主题设置，将主题白色样式迁移至组件[Popover](/#/components/popover) (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除属性 `mode` ，文字提示 2.0 起 不再支持模式设置，将模式设置迁移至组件[Popover](/#/components/popover) (by [@HXCStudio123](https://github.com/HXCStudio123) )
  - 移除事件 `menu-click` 该事件已迁移至组件[Popover](/#/components/popover) (by [@HXCStudio123](https://github.com/HXCStudio123) )

#### Bug 修复

- Checkbox
  - 修复复选框组禁用模式下，单项禁用失效问题 (by [@HXCStudio123](https://github.com/HXCStudio123) )

### 1.5.1

*2020-05-18*

#### Bug 修复

- Swipe
  - 修复只有1项时的滑动异常 (by [@yawuling](https://github.com/yawuling) )

#### 优化

- Doc
  - 优化文档的响应式 (by [@yawuling](https://github.com/yawuling) )

### 1.5.0

*2020-05-13*

#### 新特性

- Checkbox
  - 支持复选框组下的单个复选框触发 `change` 事件 (by [@yawuling](https://github.com/yawuling) )
- Swipe
  - 新增属性 `animate` (by [@yawuling](https://github.com/yawuling) )

#### Bug 修复

- Toast
  - 修复文案过长不换行导致超出页面的问题 (by [@yawuling](https://github.com/yawuling) )

#### 优化

- DropMenu
  - 标题修改为水平居中 (by [@yawuling](https://github.com/yawuling) )
- Doc
  - Grid 文档补全页面导航 (by [@yawuling](https://github.com/yawuling) )
  - Swipe 文档暴露 `prev`，`next`，`swipeTo` 方法 (by [@yawuling](https://github.com/yawuling) )
  - 优化文档的响应式 (by [@yawuling](https://github.com/yawuling) )
  - 添加爬虫文件sitemap，优化搜索功能 (by [@HXCStudio123](https://github.com/HXCStudio123) )

### 1.4.1

*2020-03-22*

#### Bug 修复

- 修复新组件入口文件未引入注册问题 (by [@yawuling](https://github.com/yawuling) )

#### 优化

- Doc
  - 修复 DropMenu 文档组件名错误问题 (by [@yawuling](https://github.com/yawuling) )
  - 修复 Tabs 文档组件名错误问题 (by [@yawuling](https://github.com/yawuling) )
- Demo
  - 修复 DropMenu demo 的展示 (by [@yawuling](https://github.com/yawuling) )

### 1.4.0

*2020-03-13*

#### 新特性

- Col
  - 新增组件 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- DropMenu
  - 新增组件 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Grid
  - 新增组件 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- Img
  - 新增组件 (by [@houtianfu](https://github.com/houtf) )
- Row
  - 新增组件 (by [@HXCStudio123](https://github.com/HXCStudio123) )
- SortButton
  - 新增组件 (by [@Gkxie](https://github.com/Gkxie) )
- StatusTip
  - 新增组件 (by [@RedJoy](https://github.com/RedJoy) )

#### Bug 修复

- Cell
  - 修复标签包裹问题 (by [@yawuling](https://github.com/yawuling) )
- Checkbox
  - 修正单个复选框下的change事件触发和入参 (by [@yawuling](https://github.com/yawuling) )
- Picker
  - 修复多级联动，修改内部值后取消恢复数据源； (by [@yawuling](https://github.com/yawuling) )
  - 修复 column-change 异步情况下无法准确获取值的问题 (by [@yawuling](https://github.com/yawuling) )
- PickerView
  - 修复columns为空数组情况下的内存溢出 (by [@yawuling](https://github.com/yawuling) )
- Slider
  - 修正slider样式 (by [@yawuling](https://github.com/yawuling) )
- Search
  - 高度问题修复 (by [@HXCStudio123](https://github.com/HXCStudio123) )

#### 优化

- Doc
  - 自定义主题 (by [@yawuling](https://github.com/yawuling) )
  - 新增Col/Row组合使用Layout文档 (by [@HXCStudio123](https://github.com/HXCStudio123) )

### 1.3.0

*2020-02-11*

#### 新特性

- Cell
  - 新增属性`size`, `title-width`, `center`, `replace` (by [@yawuling](https://github.com/yawuling) )
- Checkbox
  - 新增属性`inline` (by [@yawuling](https://github.com/yawuling) )
- DatetimePicker
  - 新增属性`size`, `label-width`, `error`, `align-right` (by [@yawuling](https://github.com/yawuling) )
  - 添加与 CellGroup 组件的关联 (by [@yawuling](https://github.com/yawuling) )
- Input
  - 新增属性`label`, `label-width`, `size`, `error`, `center` (by [@yawuling](https://github.com/yawuling) )
  - 新增插槽`label` (by [@yawuling](https://github.com/yawuling) )
  - 添加与 CellGroup 组件的关联 (by [@yawuling](https://github.com/yawuling) )
- Picker
  - 新增属性`size`, `label-width`, `error`, `align-right` (by [@yawuling](https://github.com/yawuling) )
  - 添加与 CellGroup 组件的关联 (by [@yawuling](https://github.com/yawuling) )
- Radio
  - 新增属性`inline` (by [@yawuling](https://github.com/yawuling) )
- SwipeAction
  - 新增组件 (by [@Gkxie](https://github.com/Gkxie) )
- Tag
  - 新增属性`dynamic`，支持新增标签操作 (by @awjing )

#### Bug 修复

- Search
  - 修复关闭时内部值未还原的问题 (by [@yawuling](https://github.com/yawuling) )
- Picker
  - 修复value为空时选择第一项失败的问题 (by [@yawuling](https://github.com/yawuling) )
- PickerView
  - 修复value为空时选择第一项失败的问题 (by [@yawuling](https://github.com/yawuling) )
- Checkbox
  - 修复map功能的样式在不同屏幕尺寸的展示问题 (by [@yawuling](https://github.com/yawuling) )
- Tooltip
  - 修复map功能的样式在不同屏幕尺寸的展示问题 (by [@yawuling](https://github.com/yawuling) )

#### 优化

- Checkbox
  - 优化 button 类型复选框选中样式 (by [@yawuling](https://github.com/yawuling) )
- Doc
  - 文档支持响应式布局 (by [@yawuling](https://github.com/yawuling) )
  - 新增Form表单组合使用文档 (by [@yawuling](https://github.com/yawuling) )
  - 新增搜索功能 (by [@HXCStudio123](https://github.com/HXCStudio123) )

### 1.2.0

*2020-01-06*

#### New features

Picker

- 添加 `before-confirm` 属性

DatetimePicker

- 添加 `before-confirm` 属性

### 1.1.0

*2019-12-31*

#### New features

Sticky
- 新增粘性布局组件

InfiniteLoad
- 新增 `reset` 重置方法，重置加载状态

### 1.0.1

*2019-12-27*

#### Bug fixes

Input
- 修复 show-word-limit 功能 value 为 null 的边界问题

DatetimePicker
- 修复 display-formatter 初始值为空的边界问题

### 1.0.0

*2019-12-26*

- 增加35个组件