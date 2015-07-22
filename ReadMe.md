BoardTalk
=====================================

BoardTalk是哈尔滨工业大学微软技术俱乐部小白计划2015年度暑期项目的一个子项目，
它的目标是开发出一个新形式的微社区平台网站。

在BoardTalk中，board是用户群的基本单位，drawer是内容的组织单位，card是内容的
最小单位。

Board
-------------------------------------

从内容角度来看，Board是一系列drawer的集合；从用户角度看，Board是一群用户的集合。

一个Board下面有三类用户，分别为BoardMaster、BoardManager和BoardMember。BoardMember
可以添加新的card、评论board内的所有card以及删除自己的card；BoardManager可以批准
加入board的申请、删除其他人(不包括BoardMaster)的card、禁言指定的用户某段时间等。
BoardMaster在每个Board中是唯一的，拥有最高级别的权限，可以任免BoardManager、添加删除
合并Drawer、编辑修改Board介绍与头像、委任其他人为BoardMaster、删除本board、更改
Board访问权限等。

Board可以有三种访问方式：public, protected, private。Public board可以由名字与board ID
两种方式进入，非成员可以看到所有的card信息；protected board 只能由board ID进入，非成员
只能看到有限个card的标题。private board只能由board成员邀请才能进入查看。

Drawer
-------------------------------------

Drawer是card的组织单位，其形式可由BoardManage任意指定。Drawer支持合并操作，将两个
Drawer合为一个。合并时，可以选则按时间插入、插入到最前、插入到最后等不同方式。Drawer
控制着Board上Card的显示方式。Card分为static与dynamic两类。static Card固定置顶。而dynamic 
Card则依照Drawer的不同设置有不同的排列方式，如：按新建card时间排列、按最新回复排列、按
随机顺序排列等多种模式。

Card
-------------------------------------

Card是内容的最小单位。有权限的用户可以再Drawer中添加新的card，也可以查看其它的card
并评论回复(为了引导用户短小简洁的聊天，评论有140字的字数限制)。除了在Board中查看之外，
用户在自己的页面上也能够看到自己过去发过的所有card。另外，用户如果关注了某个card。也
会在自己的页面上看到相关信息

Timeline
-------------------------------------
除了Board页面的交互之外，网站还提供了timeline的交互方式。用户在timeline上面，可以看到
自己所在的Board里的新card，也可以看到其他人对自己的回复、站内的私信、关注的card下面的
新回复与评论等其他信息。

以上。


开发者
-------------------------------------

张翔熙: zxx_1996@qq.com

李沅泽: bbsliyuanze@163.com