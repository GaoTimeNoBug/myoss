## Android四大组件

1. Activity

   1.  生命周期

   ​      onCreate:  第一创建时调用 第一个方法 可以做初始化工作   如: setConentView 加载页面发view   初始化Activity的所需数据

   ​                         onCreate()方法中的Bundle对象 回复异常情况下的Activity的结束状态

   ​      onStar():   Activity正在被启动 即将开始  表示已经Activity已经被创建了没有开始没有在前台显示 无法与用户交互 

   ​                      可以理解为 Activity已经被显示但是看不到

   ​    onResume: 表示Activity已经可以被看见了 出现在了前台  和onStar() 对比    onStar(): 表示Activity在后台  onResume: 显示到了                        

   ​                      前台

      onPause()  :   暂停 表示正在停止  仍可见 正常情况下 紧接着onStop就会被调用    特殊情况下 快速回到当前的Activty

   ​                          那么onResume()就回被调用  (极端情况下)   onPuase()不可以进行耗时操作 会影响到activity的显示 必须执行完                     

   ​                         onPause()     新的Activity的onResume才会执行

      onstop():    表示activity停止  不可见 位于后台  可以做简单的回收工作 不可以做耗时操作

      onRestar:  

    

   

   

2. 