
## AppReview Cases:

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







[case1_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case1/1.png
[case2_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case2/1.png
[case3_1]: https://github.com/github-xiaogang/AppReview/blob/master/resource/case3/1.png


