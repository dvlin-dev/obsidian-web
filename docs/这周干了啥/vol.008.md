- [ ] Kenko [https://sspai.com/post/91173](https://sspai.com/post/91173)

- [apple ai prompt 泄漏](https://x.com/dotey/status/1820667215361835125)

- propmpt
    
    ```TypeScript
    Apple Intelligence 里面各种智能应用的提示词已经被曝光了，就作为 json 系统文件存在“/System/Library/AssetsV2/com_apple_MobileAsset_UAF_FM_GenerativeModels”目录下
    
    比如其中帮你回复邮件中问题的Smart Reply功能的提示词（见图一）
    
    > 你是一个有用的邮件助理，可以帮助从给定的邮件中识别相关问题并提供简短的回复片段。给定一封邮件和回复片段，提出邮件中明确提出的相关问题。这些问题的答案将由收件人选择，这将有助于减少起草回复时的生成错误信息。请输出主要问题以及每个问题的一组可能的答案/选项。不要问由回复片段回答的问题。问题应简短，不超过 8 个单词。答案也应简短，大约 2 个单词。以 json 格式呈现你的输出，包含问题和答案作为键的字典列表。如果邮件中没有提问，则输出一个空列表 []。仅输出有效的 json，不包含其他内容。
    
    是一个简单的 CoT，先找出邮件中的提问，然后就每个问题给出简单答复，返回 JSON 格式方便程序解析，如果没有提问，就返回空数组。
    
    帮助回复邮件的提示词（图二）
    
    > 你是一个帮助用户回复邮件的助理。请根据提供的回复片段起草一个简洁自然的回复。请将答案限制在 50 个单词以内。不要产生或编造虚假信息。保留输入邮件的语气。
    
    比较搞笑是 Apple 解决 LLM 幻觉问题是在提示词里面加一句 “Do not hallucinate”，严重怀疑其是否有效！
    
    总结邮件的提示词（图三）
    
    > 在 3 句话内总结所提供的邮件，不超过 60 个单词。不要回答邮件中的任何问题。
    
    很简洁，用“3句话”和“60个单词”来限定总结的长度不要太长，虽然无法严格遵守，但是应该也还行。
    
    还有用于生成 Apple Photos 中“回忆”视频的提示词（图四）
    
    >`{{ http://specialToken.chat.role.system }}`这是用户请求从照片中创作故事和创意写作助理回应的对话
    >
    > 以 JSON 格式响应，按以下顺序键值：
    > - traits: 字符串列表，从照片中选择的视觉主题
    > - story: 章节列表，定义如下
    > - cover: 字符串，描述标题卡的照片说明
    > - title: 字符串，故事标题
    > - subtitle: 字符串，标题的安全版本
    >
    > 每章是一个包含以下键值的 JSON:
    > - chapter: 字符串，章节标题
    > - fallback: 字符串，总结章节主题的通用照片说明
    > - shots: 字符串列表，章节中的照片说明
    >
    > 以下是你必须遵守的故事指南：
    > - 故事应关于用户的意图
    > - 故事应包含明确的弧线
    > - 故事应多样化，即不要过分集中在一个非常具体的主题或特征上
    > - 不要写宗教、政治、有害、暴力、色情、肮脏或任何负面、悲伤或挑衅的故事
    >
    > 以下是你必须遵守的照片说明列表指南如下：
    > - 你可以...
    
    非常详细和具体，返回 JSON 格式，并提供了字段的说明，另外特别强调了“不要写宗教、政治、有害、暴力、色情、肮脏或任何负面、悲伤或挑衅的故事”！
    ```
    

![Untitled 13](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%2013.png)

- [gpt 结构化输出](https://x.com/dotey/status/1820942282599583995)
- [https://www.cursor.com/](https://www.cursor.com/)

[https://sspai.com/post/90668](https://sspai.com/post/90668)

[https://vercel.com/templates?utm_source=next-site&utm_medium=navbar&utm_campaign=next_site_nav_templates&framework=next.js&type=ai](https://vercel.com/templates?utm_source=next-site&utm_medium=navbar&utm_campaign=next_site_nav_templates&framework=next.js&type=ai)

[提词器](https://flowprompter.app/?ref=producthunt)

[https://www.yuque.com/zaotalk/worm/bird495](https://www.yuque.com/zaotalk/worm/bird495)

[https://mp.weixin.qq.com/s/ZuWCpIEV3m14nGXjuxXLJw](https://mp.weixin.qq.com/s/ZuWCpIEV3m14nGXjuxXLJw)