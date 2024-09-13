# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# ssm656基于JAVA的校园失物招领平台的设计与实现+vue

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Tm8QeZE4a?p=55)


# 第1章 绪论
## 1.1 课题背景
二十一世纪互联网的出现，改变了几千年以来人们的生活，不仅仅是生活物资的丰富，还有精神层次的丰富。在互联网诞生之前，地域位置往往是人们思想上不可跨域的鸿沟，信息的传播速度极慢，信息处理的速度和要求还是通过人们骑马或者是信鸽传递，这些信息传递都是不可控制的，中间很有可能丢失，信息的传递水平决定了人们生活的水平。如今大家都在使用互联网软件产品，从内部管理设置计算机管理，提高内部信息化的管理水准，从外部市场也可以用计算机获取相关数据进行处理，如今各行各业已经严重依赖于计算机了。

本课题研究和开发校园失物招领平台，让安装在计算机上的该系统变成管理人员的小帮手，提高校园失物招领信息与寻物启事信息处理速度，规范校园失物招领信息与寻物启事信息处理流程，让管理人员的产出效益更高。
## 1.2 课题意义
传统处理数据，必须是一张张纸，然后处理完毕又是统计在一张张纸上面，不断的重复处理，最终有个结果给最高层作为参考，这个模式在互联网没有出现之前，是一种常见的事情，信息管理的效率提不上去，人多不一定力量大，因为人多肯定更加消耗资源，并且因为人类需要休息，需要管理，思想会不统一，会偷懒，所以人们研究出专门帮助人们计算的机器，就是计算机的前身，到了互联网时代，人们发现完全可以让程序供应商提供解决方案，自己挑选自己合适的方案来提高自己的产出比。所以在日常工作和生活中会发现各种各样方便人们的工具。

本课题研发的校园失物招领平台，就是提供校园失物招领信息与寻物启事信息处理的解决方案，它可以短时间处理完信息，并且这些信息都有专门的存储设备，而且数据的备份和迁移都可以设定为无人值守，从人力角度和信息处理角度以及信息安全角度，校园失物招领平台是完胜传统纸质操作的。
## 1.3 研究内容
本文对校园失物招领平台的设计与实现分成六个章节来说明。

第1章：研究校园失物招领平台的背景，以及开发校园失物招领平台的意义。

第2章：对开发校园失物招领平台的环境还有技术进行说明。

第3章：分析校园失物招领平台的可行性，性能，流程以及功能。

第4章：设计校园失物招领平台的功能结构，设计数据库E-R图以及对数据表的存储结构进行设计。

第5章：实现校园失物招领平台的功能并进行功能界面展示。

第6章：对系统测试进行阐述，以及对本系统部分功能进行检测。
# 第2章 开发环境与技术
本章节对开发校园失物招领平台需要搭建的开发环境，还有校园失物招领平台开发中使用的编程技术等进行阐述。
## 2.1 Java语言  
Java语言是当今为止依然在编程语言行业具有生命力的常青树之一。Java语言最原始的诞生，不仅仅是创造者感觉C语言在编程上面很麻烦，如果只是专注于业务逻辑的处理，会导致忽略了各种指针以及垃圾回收这些操作，导致出现问题需要解决的时间往往大于正常编程处理业务逻辑的时间，这些是非常浪费时间的。Java语言的创造者就考虑到如何避免这个问题，把指针处理和垃圾处理全部自动化，虽然这会损失一些性能，但是计算机硬件在性能上的发展速度是很快的，这些性能是可以忽略考虑的。并且C语言是针对硬件开发的语言，虽然执行效率高，但是随着硬件的变化或者操作系统的变更，就需要重新编写程序，造成重复劳动，只有解决重复性劳动的语言才算符合生存规律的语言。Java语言的创造者就针对C语言的缺点专门开发了Java语言。让Java语言不管是在什么样的环境里都是可以运行，因为在Java语言运行外面套了一个壳，也就是虚拟机，只要是Java虚拟机能安装的电脑都可以运行Java的程序。
## 2.2 MYSQL数据库
MySQL数据库是一种数据存放方面的专业软件，也是传统的行式数据模式，获取一些数据是先一行一行的获取，然后一行一行的显示，与列式数据库不同。行式数据库主要是处理最重要的数据逻辑部分，并且必须是有效数据，这样每一处的数据关联都是不可损坏，对数据安全要求比较严格还是用MySQL数据库比较好。列式数据库的发明仅仅是因为读取效率高，但是也就仅仅如此罢了。MySQL虽然比起Oracle或者SQL Server来讲，安装包只是几十兆甚至几百兆，有点小，但是功能并不会弱到哪里，严格遵循SQL标准语法。MySQL的数据存放形式从大向小的说是数据库最大，然后是表，每个表里面存放数据是有一定的规则的，数据存放是表格形式的，也就是说有横也有竖，横着的为行，一般表示一条数据，表与表之间还可以进行关联，进行分表操作，如果一条数据相关项目属性太多，那么可以把有效的相关联系做成关联，可以设定是否唯一。
## 2.3 IDEA开发工具
IDEA是捷克共和国的Java程序员开发人员创造的一个开发软件，刚开始主要是对于用Eclipse软件他们用得不顺手，所以直接开发了这款软件。之所以不顺手原因在于没有代码提升功能，原因是Eclipse只是把代码提示作为一种插件形式的存在，如果有些程序开发人员不清楚代码提示插件可能会出问题，并且代码提示只是用来作为插件，所以功能上有所欠缺。IDEA不仅仅代码提示做的很好，在代码重构上面更上如虎添翼，程序开发人员可以选择一段代码然后IDEA就会对代码进行分解重构，有效的把代码弄得更够层次感，复用性更高，用着更简洁和方便，大大的减少了代码工作量，提升了代码开发效率。当然，IDEA对于使用者这么好，肯定也是有目的的，原因在于插件越多越友好，就需要花费大量的金钱来使用，所以说IDEA使用主要是看自己喜好。
## 2.4 SSM框架
开发一个业务逻辑比较简单的应用，采用这几年最广为流传的SSM框架是很合适的。SSM框架就是Spring MVC框架和Spring框架，以及持久层常用的MyBatis框架。

三个框架有三个不同的作用。普通用户一般都是操作浏览器进行浏览自己喜欢的内容，而显示或者提交，都会被Spring MVC框架进行拦截和处理，进入到更深的一个层次就是控制层，它会智能的匹配提交的路径，对不同的来源匹配不同的处理逻辑，让不同的代码进行执行，如果只是判断用户输入信息格式的问题是不用传入到后台就可以被前端框架处理的，如果需要与数据库内容进行交互，就会从Java的POJO对象通过MyBatis自动转换数据库对应字段的数据类型，具体是该增删改查还是其他操作，都会通过MyBatis进行处理，处理结果是反馈给控制层，然后通过控制层再提交给视图层，反馈到用户希望看到的结果。

# 第3章 系统分析
本文作者在确定了研究的课题之后，从各大数字图书馆下载文献来阅读，并了解同类型的网站具备的大致功能，然后具体事务具体分析，得出本系统要研究的具体功能与性能。虽然分析系统这一阶段性工作主要是确定功能，但它却影响着后面系统开发环节的进展，系统分析这个环节是不能少的。
## 3.1 可行性分析
从三个不同的角度来分析，确保开发成功的前提是有可行性分析，只有进行提前分析，符合程序开发流程才不至于开发过程的中断。
### 3.1.1 技术可行性
在技术实现层次，分析了好几种技术实现方法，并且都有对应的成功案例，也有很多开源模块可以进行参考，所以从技术可行性分析来讲，实现校园失物招领平台是没有问题的。
### 3.1.2 经济可行性
对于身为学生的开发者而言，在经济资源上面可用者很少，为了开发校园失物招领平台，通过开发软件对硬件的要求，发现自己的电脑是完全能用来开发的，并且学校机房的配置也可以达到要求。最重要的是选择的技术都可以在网上找到不花钱的教程以及资料，因为不花钱，所以经济方面是具有可行性的。
### 3.1.3 操作可行性
校园失物招领平台的具体实现，本身参考人类的正常操作逻辑，把常用的操作习惯当做主要的导航实现，可以让使用者更快速的理解并且上手操作，实现符合逻辑的操作流程是操作可行性的具体体现。

以上就是从不同的角度来分析，确保了校园失物招领平台的正常开展。
## 3.2 系统流程
校园失物招领平台投入使用后，使用者如果能看到相应的流程操作图会提高程序的理解能力。
### 3.2.1 操作流程
使用者在操作校园失物招领平台中，应该按照本系统提供的操作流程（图3.1即为本系统的操作流程图）进行操作，可以减少操作失误，从而节省进入校园失物招领平台的时间。

![](/md/blog.001.png)

图3.1 系统操作流程
### 3.2.2 登录流程
校园失物招领平台通过登录功能（图3.2即为其登录的流程）引导使用者进入指定的功能操作区，也避免非本系统的用户享受本系统提供的服务以及查看本系统提供的信息，进而保证用户安全。

![](/md/blog.002.png)

图3.2 登录流程
### 3.2.3 删除信息流程
校园失物招领平台在经过长期使用后，会产生很多的数据信息。为了腾出存储空间存放更多的数据，本系统数据库中存储的数据，一些没有参考价值的数据需要进行删除（图3.3即为删除信息的流程），删除数据过程中，为避免误删，使用者要根据系统的提示来决定是否删除数据。

![](/md/blog.003.png)

图3.3 删除信息流程
### 3.2.4 添加信息流程
校园失物招领平台提供可视化的功能操作区，非常方便使用者进行数据操作，当使用者往系统中录入数据时（图3.4即为添加信息的流程），本系统也会进行数据合法性的判断，符合要求的数据才能够在数据库指定表中进行登记。

![](/md/blog.004.png)

图3.4 添加信息流程
## 3.3 性能需求
需求分析少不了对项目用到的硬件设备进行分析，这样才符合正常的分析流程。只谈功能需求不谈性能需求，是一件很严重的事情，可能会导致一些不可控的问题出现。

以下从这几个角度来分析系统性能。

(1)系统数据的容量：从数据角度来分析，每个表和每个数据库，达到的数据量到一定的程度，是否需要分表或者是分库，超过了数据的设定限度，可能会导致数据反映迟钝，容错量增加。

(2)数据精度的要求：需要对需求分析里面数据设定环节，考虑相应的数据精度问题，需要发现数据是常用的精度还是非常用的精度，进而设定不同的数值。

(3)时间响应要求：从用户提交操作，到页面反映，中间有个数据处理的问题，需要考虑预测数据量的大小，提前预案分库分表的设计，数据量再大就要考虑增加列式数据库的问题，这些都不是一拍脑门就能决定的，都需要经验和同行业的数据分析研判，才能符合用户的要求，毕竟响应时间太久操作起来也不舒服。

(4)普适性问题：用户使用应该不需要感知服务端的数据量问题或者响应问题，只需要任意一台电脑，不需要更多的操作，打开浏览器就能用，太多的设置以及操作，不符合普适性操作。

(5)页面设计问题：功能符合要求之后，肯定是要丰富页面的。页面设计才是用户长时间面对的问题，首先考虑数据的整洁性，让页面看起来更加的清爽。颜色与数据方面，该不同颜色就不同颜色，降低用户长时间使用出现的视觉疲劳，让用户使用起来心情不至于太差。

(6)系统的稳定性：正常用户操作系统页面，必须是该提交提交，正常输入符合逻辑，不能随随便便的就出各种问题，导致用户操作疲惫，并且输入的数据和回显的数据符合用户的要求。如果正常操作都会出现问题，那设计就是不稳定的，这一点肯定不行。只要是与数据进行交互的系统，都必须稳定。系统稳定从开发部署角度上来分析，可以考虑数据的冗余备份功能，自动值守功能，机房数据同步，机房分开的功能，这些都可以让系统的稳定性得到提升。

系统的性能需求需要对业务很熟练的情况下判断然后分析，再从系统性能需求来逐条实现，可以让设计的系统有使用价值。
## 3.4 功能需求
校园失物招领平台根据使用权限的角度进行功能分析，并运用用例图来展示各个权限需要操作的功能。

图3.5即为管理员用例图，管理员权限操作的功能包括管理失物招领信息，管理举报反馈信息，管理寻物启事信息，管理论坛，管理公告，管理失物认领信息等。

![](/md/blog.005.png)

图3.5 管理员用例图

图3.6即为用户用例图，用户权限操作的功能包括对失物招领信息进行失物认领，发布寻物启事以及失物招领信息，查看失物认领信息，发布举报反馈信息等。

![](/md/blog.006.png)

图3.6 用户用例图
# 第4章 系统设计
用户对着浏览器操作，肯定会出现某些不可预料的问题，但是不代表着系统对于用户在浏览器上的操作不进行处理，所以说，要提前考虑可能会出现的问题。
## 4.1 系统设计思想
系统设计，肯定要把设计的思想进行统一，只有统一的思想才能指导程序的开发，并且可以让众多的程序开发人员更快速的进入状态，提高开发速度。根据当前系统的既定需求，下面将进行本系统设计思想的阐述。

(1)扩展性：开发任何一个系统的时候不可避免要考虑这个问题。软件版本的更迭是一种常识，任何一个软件都不会一次性开发就成永恒，软件是一个不断成长的东西。所以考虑问题的时候需要对当前问题进行数据上的扩大化，然后进行归纳整理，最终形成具有一定扩展性的程序。程序的可扩展性必然会影响开发进度，所以最终需要综合评估程序的可扩展程度，进而有的放矢，循序开发。

(2)实用性：程序设计是一个先高屋建瓴式的设想，然后再具体化，实用性就是具体化的第一个步骤，要充分考虑使用者是不懂程序设计的这一点，使用者只是懂得常规性的上网操作步骤，并不需要对程序进行理解，所以一定要让使用者感觉到便利，感觉到实用性的存在，如果使用者使用程序过程中没发现使用程序的好处，那么程序设计的实用性将大大降低。

(3)安全性：当使用者使用的过程中，会产生大量的相关数据，这些数据必须有安全性的保证，否则当使用者发现数据出现问题的原因是程序设计问题的时候，将会对程序开发者失去信任，甚至可能会产生大量的费用赔偿问题，这是一个不可避免的问题。所以安全性关系开发与使用者双方的经济利益，程序的安全性是一定要保证的。

(4)先进性：程序设计的先进性是开发者进行考虑的，必须要在满足系统功能的前提下，必须要选择好当下最合适的技术。最合适的技术要从开发成本，使用成本以及维护成本里面综合分析，经过综合分析后要让技术实现最优解，保持先进的技术生产力。

(5)维护性：程序开发之初就要考虑以后的维护问题。维护是在程序开发完毕，已经上线可以运作，进入生产试用过程和使用过程中才会发现需要维护的必要。要通过各方面降低维护成本，不是说维护的越少就代表程序开发的越完美，程序既然是人类进行设计制造的，肯定有很多不可避免的问题产生，那么如何维护好程序的正常运作也是一门很重要的学问。
## 4.2 功能结构设计
图4.1即为设计的管理员功能结构，管理员权限操作的功能包括管理失物招领信息，管理举报反馈信息，管理寻物启事信息，管理论坛，管理公告，管理失物认领信息等。

![](/md/blog.007.png)

图4.1 管理员功能结构

图4.2即为设计的用户功能结构，用户权限操作的功能包括对失物招领信息进行失物认领，发布寻物启事以及失物招领信息，查看失物认领信息，发布举报反馈信息等。

![](/md/blog.008.png)

图4.2 用户功能结构
## 4.3 数据库设计
校园失物招领平台运行中产生的数据需要按照提前设置的存储规则进行保存，设计出一个符合项目的最优数据存储格式，因为它能减少用户的等待时间，还可以对系统的请求在最短时间内进行响应。所以，对数据库设计时，需要对功能需求进行详细的拆分，以及对业务状态的细分，然后设计具体的存储规则，保证数据库能正常运作，缩短数据处理时间，并在一定程度上降低数据冗余，节省存储空间。
### 4.3.1 数据库概念设计
实体-联系图还有一个名称即E-R图，是Entity Relationship Diagram各英文单词首字母的缩写，它这种概念模型通常用于对现实世界进行描述。同时它还是一种能够直观表达数据中实体，联系，属性的有效手段。绘制E-R图能够选择的工具也有很多，但是Office Visio 这款软件在E-R图的绘制上一般都是作为首选工具，因为它是基于可视化处理，使用它创建E-R图非常简单。使用基本的E-R图构成元素，比如椭圆，菱形，矩形，还有实线段来表达对应的信息，椭圆代表属性，即实体的特征，矩形代表实体，即数据库中的一个具体数据表，菱形代表实体中相互关系，实线段主要是完成椭圆，矩形，菱形的连接。

（1）图4.4即为用户这个实体所拥有的属性值。

![](/md/blog.009.png)

图4.4 用户实体属性图

（2）图4.5即为失物招领这个实体所拥有的属性值。

![](/md/blog.010.png)

图4.5 失物招领实体属性图

（3）图4.6即为管理员这个实体所拥有的属性值。

![](/md/blog.011.png)

图4.6 管理员实体属性图

4. 图4.7即为寻物启事这个实体所拥有的属性值。

![](/md/blog.012.png)

图4.7 寻物启事实体属性图

4. 图4.8即为上面介绍的实体中存在的联系。

![](/md/blog.013.png)

图4.8 实体间关系E-R图
### 4.3.2 数据库物理设计
本小节主要任务即是根据上述内容进行数据存储结构的设计，实体的属性就用来表示字段名称，不同的字段表示的数据类型以及取值都不相同，以及该表各个字段是否能够保持空等进行说明，设计完成一张数据表的结构之后，在保存时同样要命名，尽量选择英文名称进行命名并保存，还不容易导致系统出错。接下来就对设计的表进行简单说明。

表4.1 论坛表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|forum\_name|帖子标题|varchar(200)|是|
|yonghu\_id|用户|int(11)|是|
|users\_id|管理员|int(11)|是|
|forum\_content|发布内容|text|是|
|super\_ids|父id|int(11)|是|
|forum\_types|帖子类型|int(11)|是|
|forum\_state\_types|帖子状态|int(11)|是|
|insert\_time|发帖时间|timestamp|是|
|update\_time|修改时间|timestamp|是|
|create\_time|创建时间 |timestamp|是|
表4.2 举报反馈表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|yonghu\_id|用户|int(11)|是|
|jubaofankui\_name|举报标题|varchar(200)|是|
|yonghu\_name|举报用户|varchar(200)|是|
|jubaofankui\_text|举报内容|text|是|
|insert\_time|举报时间|timestamp|是|
|create\_time|创建时间|timestamp|是|
表4.3 公告表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|news\_name|公告名称|varchar(200)|是|
|news\_types|公告类型|int(11)|是|
|news\_photo|公告图片|varchar(200)|是|
|insert\_time|公告时间|timestamp|是|
|news\_content|公告详情|text|是|
|create\_time|创建时间 |timestamp|是|
表4.4 失物认领表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|shiwuzhaoling\_id|失物id|int(11)|是|
|yonghu\_id|认领用户|int(11)|是|
|shiwurenling\_text|认领凭证|text|是|
|shiwurenling\_yesno\_types|审核|int(11)|是|
|shiwurenling\_yesno\_text|详情|text|是|
|insert\_time|认领时间|timestamp|是|
|create\_time|创建时间|timestamp|是|
表4.5 失物招领表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|shiwuzhaoling\_uuid\_number|失物编号|varchar(200)|是|
|shiwuzhaoling\_name|物品名称|varchar(200)|是|
|shiwuzhaoling\_types|物品类型|int(11)|是|
|status\_types|物品状态|int(11)|是|
|yonghu\_id|用户|int(11)|是|
|shiwuzhaoling\_photo|物品图片|varchar(200)|是|
|shiwuzhaoling\_time|拾遗时间|timestamp|是|
|shiwuzhaoling\_dizhi|拾遗地址|varchar(200)|是|
|shiwuzhaoling\_content|详情|text|是|
|create\_time|创建时间 |timestamp|是|
表4.6 失物招领留言表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|shiwuzhaoling\_id|物品|int(11)|是|
|yonghu\_id|用户|int(11)|是|
|shiwuzhaoling\_liuyan\_text|留言内容|text|是|
|reply\_text|回复内容|text|是|
|insert\_time|留言时间|timestamp|是|
|update\_time|回复时间|timestamp|是|
|create\_time|创建时间|timestamp|是|
表4.7 管理员表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|bigint(20)|否|
|username|用户名|varchar(100)|否|
|password|密码|varchar(100)|否|
|role|角色|varchar(100)|是|
|addtime|新增时间|timestamp|否|
表4.8 寻物启事表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|wupinguashi\_name|物品名称|varchar(200)|是|
|shiwuzhaoling\_types|物品类型|int(11)|是|
|status\_types|物品状态|int(11)|是|
|wupinguashi\_photo|物品图片|varchar(200)|是|
|wupinguashi\_time|丢失时间|timestamp|是|
|yonghu\_id|用户|int(11)|是|
|wupinguashi\_dizhi|丢失地址|varchar(200)|是|
|wupinguashi\_content|详情|text|是|
|create\_time|创建时间 |timestamp|是|
表4.9 寻物启事留言表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|wupinguashi\_id|物品|int(11)|是|
|yonghu\_id|用户|int(11)|是|
|wupinguashi\_liuyan\_text|留言内容|text|是|
|reply\_text|回复内容|text|是|
|insert\_time|留言时间|timestamp|是|
|update\_time|回复时间|timestamp|是|
|create\_time|创建时间|timestamp|是|
表4.10 用户表

|字段|注释|类型|空|
| :-: | :-: | :-: | :-: |
|id (主键)|主键|int(11)|否|
|username|账户|varchar(200)|是|
|password|密码|varchar(200)|是|
|yonghu\_name|用户姓名|varchar(200)|是|
|sex\_types|性别|int(11)|是|
|yonghu\_id\_number|身份证号|varchar(200)|是|
|yonghu\_phone|手机号|varchar(200)|是|
|yonghu\_photo|照片|varchar(200)|是|
|create\_time|创建时间|timestamp|是|
![打开新的 phpMyAdmin 窗口](/md/blog.014.png "打开新的 phpMyAdmin 窗口")

![打开新的 phpMyAdmin 窗口](/md/blog.014.png "打开新的 phpMyAdmin 窗口")

第5章 系统实现

编程人员在搭建的开发环境中，会让各种编程技术一起呈现出最终效果。本节就展示关键部分的页面效果。
## 5.1 管理员功能实现
### 5.1.1 论坛管理
图5.1 即为编码实现的论坛管理界面，管理员对论坛帖子进行查看，同时可以对论坛帖子的回复信息进行查看，本界面显示的论坛帖子信息存在错误数据可以进行更改，可以删除需要删除的论坛帖子信息。

![](/md/blog.015.png)

图5.1 论坛管理界面
### 5.1.2 失物认领管理
图5.2 即为编码实现的失物认领管理界面，管理员在失物认领管理界面对已经认领的失物信息进行查询，删除，查看等。

![](/md/blog.016.png)

图5.2 失物认领管理界面
### 5.1.3 寻物启事管理
图5.3 即为编码实现的寻物启事管理界面，管理员在寻物启事管理界面具备修改寻物启事信息，新增寻物启事信息，查询寻物启事信息，删除寻物启事信息等权限。

![](/md/blog.017.png)

图5.3 寻物启事管理界面
### 5.1.4 用户管理
图5.4 即为编码实现的用户管理界面，管理员修改用户手机号，照片，用户姓名等信息，删除需要删除的用户，为用户的账号进行密码重置等。

![](/md/blog.018.png)

图5.4 用户管理界面
### 5.1.5 失物招领管理
图5.5 即为编码实现的失物招领管理界面，管理员也能在失物招领管理界面对失物招领信息进行增删改查管理。

![](/md/blog.019.png)

图5.5 失物招领管理界面
## 5.2 用户功能实现
### 5.2.1 失物招领
图5.6 即为编码实现的失物招领界面，用户可以在留言区域发布留言，可以对失物进行认领。

![](/md/blog.020.png)

图5.6 失物招领界面
### 5.2.2 寻物启事
图5.7 即为编码实现的寻物启事界面，用户在留言区域发布留言，对寻物启事详情信息进行查看。

![](/md/blog.021.png)

图5.7 寻物启事界面
### 5.2.3 在线论坛
图5.8 即为编码实现的在线论坛界面，用户通过在线论坛发帖，评论帖子等。

![](/md/blog.022.png)

图5.8 在线论坛界面
### 5.2.4 失物招领留言管理
图5.9 即为编码实现的失物招领留言管理界面，用户在失物招领留言管理界面中对留言内容进行查看并回复。

![](/md/blog.023.png)

图5.9 失物招领留言管理界面
### 5.2.5 失物招领管理
图5.10 即为编码实现的失物招领管理界面，用户可以发布并管理失物招领信息，包括更改，删除，查询自己发布的失物招领信息等。

![](/md/blog.024.png)

图5.10 失物招领管理界面

# 










