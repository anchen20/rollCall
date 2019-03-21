# rollCall
基于bootstrap3和jq的简易点名页面

## 使用帮助

### 数据导入方法

1. 点击导入“导入数据“按钮进入数据导入界面。

2. 点击”数据导入“一栏下的”选择文件“按钮。

3. 选择相应文件点击确定。批量导入时多选。

#### 导入txt文件要求

- 文件名为班级名。导入后文件名影响下拉菜单的班级选择。

- txt文件内，每一行对应一个姓名。

### 永久性写入数据

1. 按上述步骤导入txt数据

2. 导入成功后。在点名界面，确认能正常使用。在数据导入界面，点击“显示json数据按钮”。复制显示的数据。

3. 找到网页源文件“rollCall.html”，右键打开方式，以记事本打开。

4. 在记事本中，点击编辑-替换（或以快捷键Ctrl+f打开），查找“var json =”。查找到“var json =”将等号之后的数据替换为，第二步复制的数据。

5. 保存文件，退出记事本。

### 版本停止维护

由于单纯以bootstrap和jq实现，有其局限。诸多功能无法实现，或复杂实现。放弃此版本维护，研究java+html+sqlite实现