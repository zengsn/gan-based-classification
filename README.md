# 简要说明
  
这是包含了Fashion-minst和mnist的DCGAN运行框架。  
在**model文件夹**中的数据是**mnist**的数据集文件，在data中的**mnist文件夹**是**Fashion-mnist**数据集文件。  
 
# 运行 
## 基于Fashion-mnist的DCGAN框架运行

首先，分别修改**model.py**中第465、469、473及477行的代码，将os.path.join（）函数里面的路径改成你本机的mnist文件夹路径。（注意是**绝对路径**）
修改完后，按照官方文档中的命令运行即可：  
```
$ python main.py --dataset mnist --input_height=28 --output_height=28
```
输入上述命令即可运行基于Fashion-mnist的DCGAN框架。  
  
## 基于mnist的DCGAN框架运行  
  
将model文件夹中的mnist数据集文件覆盖mnist文件夹中的Fashion-mnist文件即可。  
**注意**：由于mnist数据集文件名是t10k-images.idx3-ubyte，images和idx3之间是**点**，而Fashion-mnist数据集文件名是**横杠**，  
故覆盖完后还需修改**model.py**中第465、469、473及477行的代码，将点换成横杠。  
