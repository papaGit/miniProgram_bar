# miniProgram_bar
小程序父子间传值【以自定义头部导航栏为例】

## 前言：
小程序默认是用它自身的导航栏模板的，如果想用自己自定义的导航栏，就要在app.js中设置一下属性。

![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/first.png)

## step1：创建自定义组件

* 1.1创建一个components文件夹，用于放置所有自定义的组件。
* 1.2创建一个子组件（自定义名字），与普通页面相似，也是由由 json、wxml、wxss、js 4个文件组成。

 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/1.png)
 
 阿斯顿撒多撒
## step2：子组件的配置
* 2.1【自定义组件.json】进行自定义组件声明，当component 字段设为true时，表明此组件为自定义组件。

 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/2.png)
 
* 2.2【自定义组件.wxml】在这里就可以根据自己的需求编写自定义的头部导航栏了。

 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/3.png)
 
* 2.3【自定义组件.wxss】编写自己喜欢的样式。

 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/4.png)
 
* 2.4【自定义组件.js】根据需要动态修改的数据在properties中定义好数据类型。

 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/5.png)
 
 
## step3：父组件引用子组件
* 3.1【父组件.json】在父组件中进行声明我要引入哪个组件，并给它取个名字。
 
 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/6.png)
  
* 3.2【父组件.wxml】在父组件中引入自定义的子组件。但是爸爸不是要这个名字哦，所以就关联到父子间的传值问题了，请看下一步。
  
 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/7.png)
 
* 3.3【父组件.js】在父组件中设置好导航栏的名字
 
 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/8.png)
  
* 3.4【父组件.wxml】把js设置好的值传个子组件，记得传值的格式哦！
 
 ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/9.png)
 
## 大功告成
 
  ![](https://github.com/papaGit/miniProgram_bar/raw/master/mdImg/10.png)
  
  
 
    
