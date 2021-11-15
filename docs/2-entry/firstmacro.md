# 第一个宏

## 1.(非常重要!!!)关闭macrodroid的宏

没错,怕你瞎玩写了个套娃宏,比如触发器打开屏幕,动作关闭屏幕,而你后台活的好,那这就成砖了,root后可以刷机,不Root我就不知道了,所以这非常重要,请一定要设置!!! 

### 2.新建宏

点击宏->右下角+新建一个宏

### 2.1触发器

触发器:(右上角+号添加触发器)

{电源键按下}配置为5下(你可以选别的,但是如果屏幕都开不了,没有意义)

位置:电池->电源键按下
或者搜索[电源键按下]

### 2.2动作

动作:
{禁用Macrodroid}

位置:Macrodroid特定
搜索:禁用Macrodroid

完成后点击右下角浮动按钮保存

### 2.3完成图

完整照片:

![image-20211115171846144](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/macrodroidoff.png)

### 不要忘了测试!

### 2.4启动macrodroid

![image-20211115160333405](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/macrodroidon.png)

## 3.屏幕解锁宏

屏幕锁有以下

1.无

2.滑动

3.图案

4.PIN码

5.密码

### 说明

1.无

部分手机可能还有滑动,可以到开发者选项开启不锁定屏幕,即直接开启进入桌面,对安全性无要求或者其他方式全部失败可以用这个

2.滑动

这个很简单,手势坐标滑动即可

3.图案

请换一种屏幕锁,图案解锁成功率极低

4.PIN码

这个也可以坐标点击

5.密码

可以点击输入框后粘贴密码

### 3.1实际操作
由于需要使用坐标,请打开开发者选项,打开指针位置,(不知道请百度你的机型+开发者选项)

![image-20211115162619047](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/coordinateon.png)

### 3.2滑动宏
首先坐标大家应该都知道,所以滑动也很简单
从一点到另外一个点,具体数值大家可以自己试
从下往上滑动就是x1:550,y1:2000 x2:550,y2:100
x1 y1就是滑动起始,可能你的手机比较小,那么你可以自己试,修改y数值即可
x2 y2终点坐标

弄出来就是这样

![image-20211115172427376](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/xy1.png)

完整的宏就是这样

![image-20211115172542766](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/Completemacro.png)

触发器:空触发器(搜索空触发器)待会会讲调用这个宏的方法,不然你每做一个宏就要写一次开屏幕的脚本

动作:开启屏幕(搜索屏幕)(大家自己找或者搜索吧,我就不说在哪里了)

等待2秒(搜索等待)这个是防止宏执行的太快了,上一个还没执行下一个就执行了,这样就乱套了,所以要加一个等待时间

页面交互:(搜索页面交互)选择手势即可



### 3.3PIN码宏

和3.2一样的,找到你的密码坐标,用点击即可,中间加上等待时间

![image-20211115173440803](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/PINmacro.png)

### 3.4密码宏

可以和3.3一样,依此点击坐标,也可以粘贴密码回车

![image-20211115174253545](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/passwordmacro.png)

## 调用解锁屏幕宏

好了,你已经学会解锁了,接下来教你们调用解锁宏

![image-20211115174544686](https://cdn.jsdelivr.net/gh/Goojoe/picgo/macrodroid/macrorun.png)

只需要将要解锁的宏使用宏运行动作即可,是不是超级简单,然后运行其他动作实现你想要的功能了

- [下一节>>功能](2-entry/function)