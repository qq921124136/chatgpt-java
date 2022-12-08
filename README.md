

# ChatGPT Java Api

![stable](https://img.shields.io/badge/stability-stable-brightgreen.svg)
[![Maven Central](https://img.shields.io/maven-central/v/com.github.plexpt/chatgpt)](https://maven-badges.herokuapp.com/maven-central/com.github.plexpt/chatgpt)

[English Doc](https://github.com/PlexPt/chatgpt-java/blob/main/README_en.md).


OpenAI ChatGPT 的逆向工程SDK。可扩展用于聊天机器人等。

感谢 [revChatGPT](https://github.com/acheong08/ChatGPT).

# 功能
![image](https://user-images.githubusercontent.com/36258159/205534498-acc59484-c4b4-487d-89a7-d7b884af709b.png)

![image](https://user-images.githubusercontent.com/15922823/206353660-47d99158-a664-4ade-b2f1-e2cc8ac68b74.png)


可以写代码，写小说，写作文、演讲稿、工作报告、读书笔记、合同等
# [一些有趣的玩法](./USEAGE.md)

## 使用

maven
```
<dependency>
    <groupId>com.github.plexpt</groupId>
    <artifactId>chatgpt</artifactId>
    <version>1.0.1</version>
</dependency>
```

gradle
```
implementation group: 'com.github.plexpt', name: 'chatgpt', version: '1.0.1'
```


然后
```
  Chatbot chatbot = new Chatbot("sessionToken");
  Map<String, Object> chatResponse = chatbot.getChatResponse("hello");
  System.out.println(chatResponse.get("message"));
```
### sessionToken获取
https://github.com/acheong08/ChatGPT/wiki/Setup#token-authentication

1. 通过 https://chat.openai.com/chat 注册并登录。
2. 打开浏览器开发者工具，切换到 Application 标签页。
3. 在左侧的 Storage - Cookies 中找到 __Secure-next-auth.session-token 一行并复制其值


### 注册教程

https://juejin.cn/post/7173447848292253704

https://mirror.xyz/boxchen.eth/9O9CSqyKDj4BKUIil7NC1Sa1LJM-3hsPqaeW_QjfFBc

### 也可以控制台直接使用
1. 下载
2. 编辑 config.json 里的sessionToken
3. 运行 run.bat

# Awesome ChatGPT
[My list](https://github.com/stars/acheong08/lists/awesome-chatgpt)

If you have a cool project you want added to the list, open an issue.

# Disclaimers
这不是官方的 OpenAI 产品。这是一个个人项目，与 OpenAI 没有任何关联。

### This is a library and not intended for direct CLI use
CLI 功能仅用于演示和测试。不支持验证码（对于不干净的 IP 地址）

### CLI use
[@rawandahmad698](https://github.com/rawandahmad698) has a much better CLI tool at

**[PyChatGPT](https://github.com/rawandahmad698/PyChatGPT)** supports captcha!

# Star History

[![Star History Chart](https://api.star-history.com/svg?repos=PlexPt/chatgpt-java&type=Date)](https://star-history.com/#PlexPt/chatgpt-java&Date)
