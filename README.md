# popBackGestureController
在全页面实现pop返回回弹手势，只需一行代码
###Swift用法：
在桥接文件中导入头文件    #import "PopAnimationViewController.h"
   然后在navigationController的root viewController的类文件中加入：  

 let nav = self.navigationController
 var popAnimationVC = PopAnimationViewController(navigationController: nav);
