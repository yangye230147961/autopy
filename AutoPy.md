## AutoPy
### 简介
> ``AutoPy``是为python开发者提供的一个安卓插件,由路飞大佬开发维护,主要功能为了实现使用python在安卓端完成一些操作,例如点击,滑动,返回
### 准备
> 安装`AutoPy.apk`,点击`安装模块`,开启`无障碍权限`,开启`开发者选项`中`显示指针位置`
### 测试
> 完成准备工作后,点测试按钮,测试相应功能,若功能正常,请继续后面操作,若功能无响应,则检查准备工作
### 导入
> 完成上述操作后,模块路径`/sdcard/qpython/AutoPy.py` 进入目录导入模块
```shell
$ cd /sdcard/qpython  #进入目录
$ python  #启动python
$
```
```python
>>> import AutoPy #导入模块
>>>
```
### 使用
#### AutoPy.tap(X,Y)
> 模拟点击指定位置

|参数|类型|说明|
|:-:|:-:|:-:|
|X|`int`|点击位置x坐标|
|Y|`int`|点击位置y坐标|

```python
import AutoPy #导入模块
AutoPy.tap(400,400) #点击(400,400)位置
```

#### AutoPy.swipe(x1,y1,x2,y2,t)
> 模拟滑动操作

|参数|类型|说明|
|:-:|:-:|:-:|
|x1|`int`|起始位置x坐标|
|y1|`int`|起始位置y坐标|
|x2|`int`|结束位置x坐标|
|y2|`int`|结束位置y坐标|
|t [可选]|`int`|起始位置到结束位置持续时间|

```python
import AutoPy #导入模块
AutoPy.swipe(0,0,1000,1000)#从(0,0)拖拽到(1000,1000)
```

#### AutoPy.gesturer([x1,y1,x2,y2,...,t])
> 连续滑动操作

|参数|类型|说明|
|:-:|:-:|:-:|
|x1|`int`|起始位置x坐标|
|y1|`int`|起始位置y坐标|
|x2|`int`|结束位置x坐标|
|y2|`int`|结束位置y坐标|
|...|`int`|...|
|t [可选]|`int`|起始位置到结束位置持续时间|

```python
import AutoPy #导入模块
AutoPy.gesturer(0,0,1000,1000,2000,2000) #从(0,0)拖拽到(1000,1000)再拖拽到(2000,2000)
```

#### AutoPy.capturer()
> 三指下滑截图,没有三指截图功能机型无效

```python
import AutoPy #导入模块
AutoPy.capturer()#三指下滑实现截图
```

#### AutoPy.StartServer()
> 截图服务

```python
import AutoPy #导入模块
AutoPy.StartServer()#截图服务
```

#### AutoPy.HOME()
> 模拟主页键

```python
import AutoPy #导入模块
AutoPy.HOME()#模拟主页键
```

#### AutoPy.RECENTS()
> 模拟多任务键

```python
import AutoPy #导入模块
AutoPy.RECENTS()#模拟多任务键
```

#### AutoPy.BACK()
> 模拟返回键

```python
import AutoPy #导入模块
AutoPy.BACK()#模拟返回键
```

##### 更多功能持续开发中......
##### QQ群:540717901