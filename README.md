1. 内存管理项目,包含源码,设计报告,可执行程序。

2. 可执行程序在文件夹memoryProject中,里面包含了项目jar包,jre1.8,可执行程序，直接双击运行可执行程序即可。如果报错，请进行相应的java环境配置或者直接把源码放入IDE中运行。

3. 本项目是采用java语言开发的，通过命令行互动的内存管理项目。主要分为2个包(dynamic,request)和一个主类MainTest。通过主类的main函数选择相应的算法进行模拟。

      其中的dynamic包主要是完成对动态分区分配的模拟，他有两个子包，一个是存储实体的domain包，里面包括了要执行的作业（Task类），以及空闲分区链中的每一项(FreeItem)。而另一个子包algorithm中，有一个类FitAlgorithm,抽取了FF和BF的整个流程里面重复的代码片段。并且他可以根据选择的参数，来决定调用首次适应算法（BF类）还是最佳适应算法（FF类）中的方法。

         而request包主要是完成请求调页方式的模拟，也有两个子包domain以及algorithm。在domain包中有两个类，PageItem类主要负责存储页表中的项，InstructionSequence则负责提供一组特定规则的随机序列，模拟指令。而algorithm包中，只有一个类requestPage，负责完成请求调页方式模拟的逻辑以及展示页面。

   (详情请参照说明文档)

   ​