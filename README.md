
## AppReview Cases:

[![Join the chat at https://gitter.im/github-xiaogang/AppReview](https://badges.gitter.im/github-xiaogang/AppReview.svg)](https://gitter.im/github-xiaogang/AppReview?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

### case 1
```
2.2  Apps that exhibit bugs will be rejected

We discovered one or more bugs in your app when reviewed on iPhone running iOS 9.1 on both Wi-Fi and cellular networks.
Specifically, we found that your app does not load any content when the "积分商城" button is tapped. Please refer to the attached screenshot/s for more information.
```
![case1_1][case1_1]

```
app存在bug，拒绝
我们app有一个“积分商城”页面，是web页面，审核时由于我们没有配置好这个页面，审核人员发现内容为空，审核人员则认为是应用bug。
```

### case 2
```
3.1 - Apps or metadata that mentions the name of any other mobile platform will be rejected

We noticed that your app contains irrelevant platform information in the marketing screenshots. Referencing third-party platforms in your app or its metadata is not appropriate on the App Store.
```
![case2_1][case2_1]

```
应用截图中包含第三方应用市场信息，拒绝
我们的应用截图中存在Android字样，之前有一次被拒也是上传截图时设计省事，状态栏直接用了安卓的状态栏，被审核到拒绝。
```

### case 3
```
3.1 -  Apps with names, descriptions, screenshots, or previews not relevant to the content and functionality of the App will be rejected

We noticed that your app's metadata includes the following information, which is not relevant to the application content and functionality:
大桐乡，www.tx365.com

And When We began the review of your app but are not able to continue because we need a demo account to fully assess your app features.
Specifically, we were unable to log into the app with the demo account credentials you provided. 
Please provide demo account details, including passwords, in the App Review Information section for your app in iTunes Connect. Please ensure that the information you provide includes any data necessary to demonstrate the functionality of your app features.
```
![case3_1][case3_1]

```
应用描述:"大桐乡，www.tx365.com" 与应用内容无关， 拒绝
我们的应用描述过于简单，不能描述app的内容。
另外我们提供的demo账号有误，审核人员登录不成功，也会导致元数据拒绝。
```

### case 4
```
14.3 - Apps that display user generated content must include a method for filtering objectionable material, a mechanism for users to flag offensive content, and the ability to block abusive users from the service


14.3 Details

Your app enables the display of user-generated content but does not have the required precautions in place.

Specifically, your app does not include the necessary "Blocking" (屏蔽/黑名单) mechanism for users.

Unlike "Reporting" (举报), "Blocking" (屏蔽) allows a user to block another user, so that the user has an immediate solution to stop further harassment or other interaction from the other user. This feature addresses the user's needs while waiting for your moderators to respond to a report, or in the event the user is personally offended by posts from a specific user, but your moderators have determined the content were not against your policy.
```
![case4_1][case4_1]

```
应用中有用户产生内容，但缺少预防机制；
拒绝原因是说我们app没有屏蔽/黑名单功能，而不仅仅是举报。他这里说的屏蔽/黑名单指的是将某一用户屏蔽后，自己就不会看到该用户发布的内容。
解决办法：应用中添加屏蔽/拉黑功能。
```

### case 5
```
2.2 - Apps that exhibit bugs will be rejected

2.2 Details

We discovered one or more bugs in your app when reviewed on iPhone running iOS 9.3.2 on both Wi-Fi and cellular networks.

1. The app does not load any content under all 5 tabs using IPv6 network. 

Next Steps

Please run your app on a device to identify the issue(s), then revise and resubmit your app for review. 

Apps are reviewed on an IPv6 network. Please ensure that your app supports IPv6 networks, as IPv6 compatibility is required.

For additional information about supporting IPv6 Networks, please refer to Supporting iPv6 DNS64/NAT64 Networks.

For a networking overview, see About Networking.
```

![case5_1][case5_1]

```
应用存在bug：需要支持IPv6。

这是一个意外，我们客户服务器在审核期间域名解析存在问题，用移动4G网络访问时提示[Invalid Host]，审核人员测试时我们域名解析问题刚好存在问题，被拒绝。
刚开始查找问题的时候发现第三方即时通信通信环信库最近更新版本支持IPv6，后面看审核截图才发现不是这个问题。

```

### case 6
```
Performance - 2.1
We discovered one or more bugs in your app when reviewed on iPad and iPhone running iOS 9.3.2 on Wi-Fi.
- An error message appeared at launch for not connecting to server.
Apps are reviewed on an IPv6 network. Please ensure that your app supports IPv6 networks, as IPv6 compatibility is required.
```

![case6_1][case6_1]

```
苹果审核要求应用支持IPv6，之前一直以为是App问题，参考苹果提供的方法模拟了ipv6环境测试没有问题，结果连续提交，连续被拒。后面就考虑可能是App服务器不支持ipv6，结果在服务器上运行ifconfig，发现还真没有ipv6地址。
后面参考了 http://elkpi.com/topics/aliyun-enable-ipv6.html （我们服务器是阿里云的CentOS），开启服务端的ipv6

```




[case1_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case1/1.png
[case2_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case2/1.png
[case3_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case3/1.png
[case4_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case4/1.png
[case5_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case5/1.png
[case6_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case6/1.png


