# 钉钉签到提醒

本文主要介绍如何使用使用现成的免费软件快速实现简单的钉钉自动签到功能,步骤非常设置于无需任何编程基础的小白也能轻松实现定时自动打卡.

通过本节课程,你将学习到以下内容:

- 怎么开启钉钉极速打卡功能;
- 如何唤醒手机中的知名软件;
- 如何自己给自己发推送提醒;
- 如何运行24h不间断定时程序.

## 本节目录大纲

{% simplemindmap style={"height":"350px"} %}
```markdown
- 钉钉签到提醒
    - 前言
    - 原理
        + 极速签到
        + URL Scheme
        + 定时唤醒
    - 实现
        + 钉钉设置
        + 唤醒链接
        + 定时唤醒
    - 总结
```
{% endsimplemindmap %}

<!-- toc -->

## 前言

**关键词**

```mardown
+ 忘记签到
+ 快速签到
+ 提醒签到
```

现如今钉钉已经成为全国性的 app,不仅工作中的上班族正在使用,连小学生也不放过,直播网课大多数首选钉钉,不得不说钉钉真的是让人又爱又恨!

最简单也是个人使用频率最高的的打卡签到功能让我忍不住吐槽,打卡签到提醒方式只有两种还是单选,要么设置闹钟要么设置极速打卡!

![dingtalk-reminder-setting-preview.png](./images/dingtalk-reminder-setting-preview.png)

简单流程如下:

```mermaid
graph LR
    拿出手机-- 心里盘算时间 --> 打开钉钉 -- 快捷入口/极速打卡 --> 打卡签到
```

上述流程中让我觉得不爽的是每次打卡都要**自己心里盘算着打卡时间**,所以有时候可能就会忘记,错过了打卡时间,事情虽然小但需要浪费脑容量未免有些伤神,因此需要一种更加傻瓜式操作流程来解放大脑,让我沉浸在工作中吧!


