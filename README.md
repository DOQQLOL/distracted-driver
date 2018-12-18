# distracted-driver

项目使用Jupyter notebook 作为开发环境，在google的Colab上训练模型。
Colab上集成了项目主要使用的tensorflow，keras，numpy，pandas，matplotlib，glob等模块，无需额外配置。
个人电脑上安装Anaconda软件，编程环境参照优达学成的课程内的教程配置tensorflow/python3.6；需手动安装的模块可以通过conda/pip install ~ 来安装；可采用清华镜像。

方法一：数据增强训练模型，采用模型融合，融合VGG16、VGG19、xception三个模型，最后得分0.26996.
其中，
VGG16模型训练时间：5885s；
VGG19模型训练时间：8282s；
xception模型训练时间：18087s；
总共训练时间8.9小时。

方法二：采用K折验证训练模型
VGG16模型训练时间：16小时。
