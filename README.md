# BlurEffectMenu
仿钉钉的毛玻璃弹出菜单，比较简单的实现，代码有注释。

#使用方法：

    BlurEffectMenuItem *addMattersItem=[[BlurEffectMenuItem alloc]init];
    [addMattersItem setTitle:@"添加事项"];
    [addMattersItem setIcon:[UIImage imageNamed:@"addMatters"]];
    
    BlurEffectMenuItem *addSchedulesItem=[[BlurEffectMenuItem alloc]init];
    [addSchedulesItem setTitle:@"添加日程"];
    [addSchedulesItem setIcon:[UIImage imageNamed:@"addSchedule"]];
    
    BlurEffectMenuItem *setupChatItem=[[BlurEffectMenuItem alloc]init];
    [setupChatItem setTitle:@"发起会话"];
    [setupChatItem setIcon:[UIImage imageNamed:@"setupChat"]];
    
    BlurEffectMenuItem *searchContactsItem=[[BlurEffectMenuItem alloc]init];
    [searchContactsItem setTitle:@"查找联系人"];
    [searchContactsItem setIcon:[UIImage imageNamed:@"searchContacts"]];
    
    
    BlurEffectMenu *menu=[[BlurEffectMenu alloc]initWithMenus:@[addMattersItem,addSchedulesItem,setupChatItem,searchContactsItem]];
    [menu setDelegate:self];
    menu.modalPresentationStyle = UIModalPresentationOverFullScreen;
    [menu setModalTransitionStyle:UIModalTransitionStyleCrossDissolve];
    [self presentViewController:menu animated:YES completion:nil];



#BlurEffectMenu Delegate

    //点击背景dismiss
    - (void)blurEffectMenuDidTapOnBackground:(BlurEffectMenu *)menu;

    //点击每个item
    - (void)blurEffectMenu:(BlurEffectMenu *)menu didTapOnItem:(BlurEffectMenuItem *)item;


#效果图：

   ![image](https://github.com/shenAlexy/BlurEffectMenu/blob/master/BlurEffectMenu/BlurEffectMenu/BlurEffectMenu.gif)


#联系我
   微信公众号:  iOSDevTeam
   
   Email: shenguanhua123@gmail.com
   
   [我的博客](http://blog.csdn.net/shenguanhua)  

