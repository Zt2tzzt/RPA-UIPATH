# 基础篇-控制流程之 switch 语句

## 一、切换是什么

一种流程控制语句，根据特定表达式的值，执行多组语句中的一组。

如果需要处理 3 种或 3 种以上可能的操作过程，则可以使用 switch 切换语句，而不是 if 条件语句

通过条件判断，来实现多个操作过程，只不过，条件不是布尔值，而是多个值。

具体应用场景：

- 根据申请表格的状态（草稿，已提交，批准，驳回）做相应处理。
- 根据账单的状态（未处理，处理中，已处理）做相应的处理。
- 根据员工状态（在职，离职，停薪留职）做相应的处理。
- 根据收据的年份，放到相应的文件夹
- ...

## 二、案例实践

实例：根据学员输入的成绩（A， B， C，D），显示不同的评语。

建立一个新的流程 `4 切换 学员评语`。

在序列中，加入一个输入对话框，搜索关键词 ”input“

对话框标题设置为：`"学生成绩"`；

输入标签设置为：`"请输入你的成绩"`；

输入类型设置为：多选；

输入选项设置为：`"A;B;C;D"`

> 注意：这里使用了输入对话框的“多选”

已输入的值设置为：一个新的变量 `result`，类型暂时保留 String 不变。

---

在序列中，加入一个 switch 切换，或者搜索关键词 ”switch“

表达式设置为：变量 `result`，在右侧的属性栏，将 TypeArgument 改为 String

设置一个 Case `A`

在该 case 的处理框中，放入消息框，或搜索关键词 “MessageBox”

Text 中设置为：`"优秀！"`

设置一个 Case `B`

在该 case 的处理框中，放入消息框，或搜索关键词 “MessageBox”

Text 中设置为：`"良好！"`

设置一个 Case `C`

在该 case 的处理框中，放入消息框，或搜索关键词 “MessageBox”

Text 中设置为：`"及格！"`

---

运行项目
