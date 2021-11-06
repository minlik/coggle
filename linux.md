### Linux 基础使用

[文档地址](https://shimo.im/docs/dumrsexTRJkqSgIC/read)

#### 打卡汇总

| 任务名称                                     | 难度  | 所需技能     |
| -------------------------------------------- | ----- | ------------ |
| 使用命令行登录指定的 Linux 环境              | 低、1 | ssh          |
| 在目录下创建文件夹、删除文件夹               | 低、1 | rm、mkdir    |
| 在目录下下载文件、阅读文件                   | 低、1 | wget、nano   |
| 在目录下使用 vi 或 vim 编辑文件              | 中、2 | vi、vim      |
| 在目录下创建 py 文件，并进行运行             | 中    | python       |
| 在目录下创建 py 目录，并进行 import 导入     | 中    | python       |
| 在Linux系统中后台运行应用程序，并打印日志    | 中    | nohup        |
| 使用 grep 和 awk 从文件中筛选字符串          | 高    | grep、awk    |
| 在目录下创建 zip 和 tar 压缩文件，并进行解压 | 中    | zip、tar     |
| 使用 find 和 locate 定位文件                 | 低    | find、locate |

#### 任务1：使用命令行登录指定的Linux环境

- 使用 ssh 登录系统

````sh
ssh coggle@139.198.15.157
````

#### 任务2：在目录下创建文件夹、删除文件夹

- 在 /home/coggle 目录下，新建一个以你英文昵称（中间不要有空格哦）的文件夹A

```sh
mkdir kuan
cd kuan
```

- 在文件夹A内部创建一个以 coggle 命令的文件夹B

```sh
mkdir coggle
cd coggle
```

- 在B文件夹内创建一个空 txt 文件

```sh
touch empty.txt
```

- 删除步骤4创建的文件

```sh
rm empty.txt
```

- 删除文件夹B，然后删除文件夹A

```sh
cd ..
rm -r coggle
cd ..
rm -r kuan
```

#### **任务3：在目录下下载文件、阅读文件**

- 步骤1：在 home 目录下，新建一个以你英文昵称（中间不要有空格哦）的文件夹A；在文件夹A内部创建一个以 coggle 命令的文件夹B

```sh
mkdir kuan
cd kuan
mkdir coggle
cd coggle
```

- 步骤2：使用 wget 命令下载 https://mirror.coggle.club/dataset/affairs.txt，到文件夹B

```sh
wget https://mirror.coggle.club/dataset/affairs.txt
```

- 步骤3：使用 head、cat、tail 命令阅读下载的文件。

```sh
head affairs.txt
cat affairs.txt
tail affairs.txt
```

- 步骤4：在命令行使用 ipython 进入 python3 环境，并使用pandas读取下载的文件。 

```sh
ipython
```

```python3
import pandas as pd
df = pd.read_csv('affairs.txt')
```

#### 任务4：在目录下使用vi或vim编辑文件

- 分别使用 Nano 和 Vim 创建 py 文件，并输入以下内容，并运行

```sh
nano test_nano.py
vim test_vim.py
python3 test_nano.py
python3 test_vim.py
```

```python3
#!/usr/bin/env python3
print('Hello World!')
```

#### 任务5：在目录下创建py文件，并进行运行

任务要点：python的os和sys系统接口，文件接口

- 步骤1：学习python下os模块处理文件和目录的函数，https://www.runoob.com/python/os-file-methods.html

- 步骤2：学习python下sys模块和传参函数，https://www.runoob.com/python3/python3-module.html

- 步骤3：在home/coggle目录下，在你英文昵称（中间不要有空格哦）的文件夹中，新建一个test5.py文件，该程序可以使用os、sys模块完成以下功能：
  - 功能1：打印命令行参数
  
  ```python
  #!/usr/bin/env python3
  import sys
  
  for arg in sys.argv:
      print(arg)
  ```
  
    - 功能2：使用os模块打印**/usr/bin/**路径下所有以m开头的文件。
  

**打卡内容：**

```python3
#!/usr/bin/env python3
import sys
import os

print('打印命令行参数')
for arg in sys.argv:
    print(arg)

print('\n使用os模块打印/usr/bin/路径下所有以m开头的文件')
for name in os.listdir('/usr/bin/'):
    if name.startswith('m'):
        print(name)
```



**任务6：在目录下创建py目录，并进行import导入**

任务要点：python代码模块化

- 步骤1：学习python模块化，https://www.runoob.com/python3/python3-module.html

- 步骤2：在/home/coggle目录下在你英文昵称（中间不要有空格哦）的文件夹中创建affairs文件夹。

- 步骤3：编写test6.py和affairs.py完成以下功能：

  - 功能1：affairs.py代码完成https://mirror.coggle.club/dataset/affairs.txt文件的读取，这里可以直接pd.read_csv('https://mirror.coggle.club/dataset/affairs.txt')来完成。这一部分建议写为函数。

  - 功能2：test6.py可以导入affairs.py代码

  - 功能3：test6.py可以进行命令行解析，输出[affairs.txt](https://mirror.coggle.club/dataset/affairs.txt)具体的第几行内容。

```Python
/home/coggle/
    你英文昵称命名的文件夹/
        test6.py
        affairs/
            affairs.py

```

实现要求：

```Python
在/home/coggle/你英文昵称命名的文件夹/目录下，可以执行：
python3 test6.py 10

没有bug，并完成第十行内容的输出。
```

**打卡内容：**

```python
# affairs/affairs.py 文件内容
import pandas as pd

file_name = 'https://mirror.coggle.club/dataset/affairs.txt'

def read_file(file_name=file_name):
    df = pd.read_csv(file_name)
    return df

# test6.py 文件内容
#!/usr/bin/env python3

import sys
from affairs.affairs import read_file

df = read_file()
arg = int(sys.argv[1])
print(df.iloc[1])

# 输入内容
python3 test6.py 10

# 输出内容
rate_marriage     4.0
age              22.0
yrs_married       2.5
children          0.0
religious         2.0
affairs           0.0
Name: 1, dtype: float64
```

