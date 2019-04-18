# DSSCkit

#### 项目介绍

这个项目用于方便的管理你的DSSC测试数据，能绘制数据并导出比较后的测试数据

支持管理的数据有：

1.Oriel IV Test Station生产的I-V数据

2.LabTracer2生成的V-t数据

3.Chi660e电化学工作站生成交流阻抗数据

4.CIMPS-PCS工作站生成的IPCE的谱图及其积分值的计算

5.岛津UV-2600漫反射谱的绘制、紫外可见光谱绘制的和能带间隙的计算

#### 使用说明

1.在“类型”的菜单里面找到你想处理的数据，点一下让它打上√

2.将测试的文件拖放到右上方的列表框中（可以一下拖拽一堆文件）

3.在“数据”那一菜单栏目中点击绘图按钮，就可以绘制清晰的图形了

你可以点击表头的项目名称就可以在图像里暂时屏蔽掉这条线了

那么问题来了，我想把数据放到其他地方，该怎么做呢？

4.那就选择“数据”菜单栏里面的导出，选择好要保存数据文件的位置数据就存储下来了

5.导出的文件是可以直接拖到Origin里作图或者是到Excle里进行数据分析的哦

6.想比较其他的项目的话可以选择“数据”菜单栏中的清空，将列表清空

7.想移除项目的话可以在列表框中先选中想删除的项目

再选择“数据”菜单栏中的移除，就可以把选中的项目移除了

#### 注意事项

1.导入的数据一定要横坐标一样啊，I-V的扫描电压一致，V-t的时间差不多，IPCE和紫外的波长一致

2.导出的eis图是带多个X轴的，做图需要指定多个X轴（因为数据文件中只有频率曲线是线性的）

#### 附加功能

1.如果要计算纯的IV曲线的参数（Jsc、Voc、Fill_Factor、Efficiency）

点击“高级”菜单里面的“计算IV相关值”，在弹出的窗口中的编辑中输入数据

数据格式是以Tab字符和换行符为分割的数据

从Origin或者Excle里面复制出来的数据就是这种格式的

第一列是电压（单位V），第二列是电流（单位A）就行了

2.如果想导出I-V数据列表(就是电流密度、开路电压、效率、填充因子那一堆)

可以先将IV数据填充到列表中(不需要作图)，接下来，点“高级”菜单栏里面的“导出I-V数据表”

就可以将你的数据以表单的形式导出，推荐把数据丢到Excle里面筛选比较

3.如果导入的数据是单个IPCE文件，可以点击“计算IPCE积分值”，计算积分电流曲线

积分结果在右下角的编辑内显示，按导出按钮可以将绘制的IPCE曲线和积分曲线导出

3.如果导入的数据是单个紫外吸收文件（不是漫反射），可以点击“计算吸收能带间隙”

在弹出的输入框中输入需要线性拟合的范围，线性拟合输入的范围，就可以得到拟合直线

线性拟合的结果在右下角的编辑内显示，包括线性拟合参数、拟合的能带间隙

按导出按钮可以将绘制的IPCE曲线和拟合曲线导出

4.使用过程中往往会出现一些错误，比如选中的是I-V但是拖进去的是V-t的数据

导入了重复的数据，或者误点按钮导出空数据

这些错误会在右下方的编辑框中提示，想清除的话，点击“高级”菜单中的清除就行了


#### 关于软件

本软件数据处理层由本人编写

图形框架由商业级开源引擎Echart编写，浏览器内核为开源的miniblink

如果有什么好的建议可以与作者交流(mail:982202733@qq.com)

另外软件的源代码也可以在这里找到

源代码仅作学习和交流，请勿做商业用途，有能力的童鞋也可以参与维护
                                                                                                   by Sean Pan
