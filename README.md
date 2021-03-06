# NotePad
* 做的工作为 <br> 
  * UI美化 <br> 
  * 修改背景颜色 <br> 
  * 按照修改的背景颜色来排序 <br> 
 <br> <br> 
#### 空主界面
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/1.png)
<br>  
在AndriodManifest.xml中，给主界面的主题改成Wallpaper，表示直接显示桌面背景
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/30.png)
#### 添加新的笔记，默认底色为白色
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/2.png)
#### 保存后主界面，记事的底色为白色,且有时间显示在下方，且根据记事的修改时间会改变
时间显示是在layout中的noteslist_item中添加一个时间的Testview
<br>![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/35.png)
<br> 通过数据库的调用，并更改时间的显示模式
<br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/29.png)
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/36.png)
<br> 最终呈现的主界面上的记事 
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/5.png)
多建几个记事
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/6.png)
<br> <br> 
### 搜索的主界面
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/7.png)
<br>创建搜索的anctivity <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/26.png)
<br>并且创建搜索的布局 <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/27.png)
<br> 在AndriodManifest.xml中注册，并且给搜索界面的主题改成Wallpaper，表示直接显示桌面背景 <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/32.png)
#### 用“O”来搜索 
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/8.png)
<br> 搜索采用的是模糊搜索 <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/25.png)
<br> <br>
#### 为笔记修改颜色
<br> 笔记一共有7个颜色，首先在NotePad契约类中添加
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/24.png)
<br> 并且预先定义好他们的数字<br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/33.png)
<br> 将颜色填充到ListView，用bindView来实现。自定义一个MyCursorAdapter继承SimpleCursorAdapter，既能完成cursor读取的数据库内容填充到item，又能将颜色填充 <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/39.png)
##### 修改颜色 
<br>记事本内修改的颜色
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/15.png)    
修改后的颜色
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/16.png)
#### 修改后主界面的背景也改变
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/17.png)
##### 多更改几个颜色，主界面的显示
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/18.png)
<br>
### 可按照色排序
<br> 先在菜单文件list_options_menu.xml中添加: <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/40.png)
<br> 再在NodeList中添加关于颜色排序的case <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/41.png)
<br> 最后界面的样式 <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/19.png)
#### 按颜色顺序排的
<br> 白色是第一 肉色第二 黄色第三 蓝色第四 绿色第五 粉色第六 紫色最后 按之前定义的数字来排序 <br>
![image](https://github.com/zimando/NotePad-master/raw/master/app/src/main/res/drawable/20.png)
