# popBackGestureController
在全页面实现pop返回回弹手势，只需一行代码
###Swift用法：
在桥接文件中导入头文件    #import "PopAnimationViewController.h"
   
   然后在navigationController的root viewController的类文件中加入如下一行代码即可：  

 let nav = self.navigationController
 
 var popAnimationVC = PopAnimationViewController(navigationController: nav);


###Objective C用法：
在navigationController的root viewController的类文件中导入头文件：    #import "PopAnimationViewController.h"
在root viewController的类扩展中加入属性：
@property (nonatomic) PopAnimationViewController *popAnimationViewController;

在viewdidload中加入：
UINavigationController * nav = [self navigationController];
    
    self.popAnimationViewController = [[PopAnimationViewController alloc] initWithNavigationController:nav];
