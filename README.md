# pad项目
  - com.babyfs.api.controller.pad.PadController
    1. 接口地址 padController.png
    2. PadController是我新建的controller类，是新建的接口，业务逻辑写的较多。babyfs-course3的         com.babyfs.courseservice.api.ComponentService和babyfs-library中的com.babyfs.library.api.controller.PadController 两个其他项目的代码，具体的改动可以看详细代码。
  - com.babyfs.api.controller.user.PadUserController
    1. 接口地址 PadUserController.png
    2. 用户注册、登录、修改手机号、更换设备的接口。主要调用的是babyfs-base的com.babyfs.userservice.api.AccountUserService  注册的话会注册到t_account表，字段type为5的用户是pad账户，pad_mobile记录的用户手机号，name保存的是pad的设备号
# babyfs-course3
 - service层代码com.babyfs.courseservice.impl.manager.component.CoursewareManager，api层 com.babyfs.api.controller.CoursewareController、op层com.babyfs.op.controller.component.CoursewareController。
# babyfs-note
   - 添加promethes监控、视频和图片更改水印、修改话题置顶的逻辑。有问题直接看代码就好。
# 推送
  - app入门课上课提醒，com.babyfs.app.primer.PrimerLessonNotifyService和com.babyfs.app.primer.HandleAppPushRecordService，发送完之后     将发送记录保存到t_app_push_record,后期启动一个任务请求极光接口获取推送结果。
  - 精品班用户上课督学提醒  com.babyfs.app.push.LessonNotify和com.babyfs.app.push.NoLessonNotify
  - 精品班用户进班提醒 com.babyfs.app.push.InClassNotifyService
  - 启萌之旅小程序 客服消息和一次性订阅消息 com.babyfs.app.push.InitiationJourneyService
  - 绘本馆开通付费会员发送消息 com.babyfs.app.consumer.library.LibraryPaymentMemberProcessor
# app首页block
  - 今日任务  com.babyfs.service.page.impl.TodayTaskHandler
  - app入门课  com.babyfs.service.page.impl.PrimerBlockHandler
  - 首页弹窗  com.babyfs.service.page.impl.HomeWindowHandler
# babyfs-app-operation
  - 这个项目做了拆分，后期暂时不需要维护
  
