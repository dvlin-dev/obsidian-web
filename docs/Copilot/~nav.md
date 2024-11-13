[https://sspai.com/post/91787](https://sspai.com/post/91787)
[cursor使用技巧](https://b23.tv/1FwYJSZ)


# Feature

- [ ] 三方模块
    
    > 参考 coze ，做功能性插件，根据用户的目标，自动选择，用户也可以二次选择

- [ ] 左侧是工作区，根据不同的工作区可以对你的文本设定不用的功能，提供一些预设，和优化的按钮，右侧是账号信息
- [ ] 联网
- [ ] 健康模块
- [ ] 语音模块
- [ ] ask me anything，但是不记忆
- [ ] 

nextauthjs

[[env]]

TODO

- [ ] [supabase 本地开发](https://document.memfiredb.com/docs/guides/cli/local-development)

[[supabase 自部署]]

[cf 技术栈 rag](https://twitter.com/tuturetom/status/1831152769144861037)

用 cursor

# UI
左右可以滑动的消息条： [Reanimated Swipeable | React Native Gesture Handler](https://docs.swmansion.com/react-native-gesture-handler/docs/components/reanimated_swipeable)
底部导航栏模糊效果：[x.com](https://x.com/aashudubey_ad/status/1704248400944955480)
底部导航栏，带点击二级菜单的：[x.com](https://x.com/Baconbrix/status/1759639968396333392)
这个库不错：[gluestack: React & React Native Components & Patterns](https://gluestack.io/)

# 架构

## 前端

- react-native、nextjs（web 端，轻量维护）
- Zustand
- 动画库：
	- [x.com](https://x.com/swmansion/status/1730247333621723424)
	- [GitHub - software-mansion/react-native-reanimated: React Native's Animated library reimplemented](https://github.com/software-mansion/react-native-reanimated)
- 
## 后端

- supabase（后续如果想支持国内用户，可以自部署
    - auth
- Cloudflare
    - d1（嵌套 prisma，自部署后面可以换 pgsql
    - r2

- supabase 做 auth，其他的数据操作都放在 Cloudflare 上( d1 + prisma orm)

([https://mp.weixin.qq.com/s/ZuWCpIEV3m14nGXjuxXLJw](https://mp.weixin.qq.com/s/ZuWCpIEV3m14nGXjuxXLJw))

- [https://github.com/Dhravya/cloudflare-saas-stack](https://github.com/Dhravya/cloudflare-saas-stack)
- tts: Xiaoxiao Multilingual 加 说话风格（让 AI 自动返回一个说话的风格

> [https://ai.azure.com/explore/aiservices/speech/voicegallery?tid=f89e82e7-dff3-489b-b535-e0b0e0fdd8e8](https://ai.azure.com/explore/aiservices/speech/voicegallery?tid=f89e82e7-dff3-489b-b535-e0b0e0fdd8e8)
> 
> ![image](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/image.png)

# TODO

- [ ] 模型选择参考，例如 embed 选择支持中文的 [https://github.com/marketplace/models](https://github.com/marketplace/models)
- [ ] 胃之书 app
    - 图片
        
        ![image 1](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/image%201.png)
        
- [ ] **Wordware使用的大模型是Claude-sonnet-3.5，基于AI搜索引擎Exa**

- 可以看看他的插件怎么写的
    
    ![image 2](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/image%202.png)
    

- [ ] Mednick [https://sspai.com/post/91127](https://sspai.com/post/91127)
- [ ] [https://github.com/enaqx/awesome-react?tab=readme-ov-file#react-native](https://github.com/enaqx/awesome-react?tab=readme-ov-file#react-native)
- [ ] UI 参考
    - [ ] [https://rauno.me/craft](https://rauno.me/craft)
    - [ ] [https://x.com/henrikruscon/status/1821475322929324078](https://x.com/henrikruscon/status/1821475322929324078)
    - [ ] mebot
    - [ ] [https://github.com/NervJS/taro](https://github.com/NervJS/taro)
- [ ] [https://github.com/datastax/ragbot-starter](https://github.com/datastax/ragbot-starter)
- [ ] RN UI：
    - [ ] [https://github.com/mrzachnugent/react-native-reusables](https://github.com/mrzachnugent/react-native-reusables)
    - [ ] [https://github.com/zerodays/react-native-gen-ui](https://github.com/zerodays/react-native-gen-ui)
- [ ] [https://sspai.com/post/91127](https://sspai.com/post/91127)
- [ ] [https://github.com/dkhamsing/open-source-ios-apps?tab=readme-ov-file](https://github.com/dkhamsing/open-source-ios-apps?tab=readme-ov-file)
- [ ] [https://github.com/jondot/awesome-react-native](https://github.com/jondot/awesome-react-native)
- [ ] [https://docs.expo.dev/versions/latest/sdk/notifications/](https://docs.expo.dev/versions/latest/sdk/notifications/)
- [ ] [https://ttsmaker.cn/](https://ttsmaker.cn/)
- [ ] app
    - [ ] ==**好东西**==[https://github.com/bluesky-social/social-app](https://github.com/bluesky-social/social-app)
    - [ ] [https://github.com/chatwoot/chatwoot-mobile-app](https://github.com/chatwoot/chatwoot-mobile-app)
    - [ ] ==**好东西，学习下标准库的用法！！**==[https://github.com/expo/expo](https://github.com/expo/expo)
    - [ ] ==**好东西但是代码不是RN**==[https://github.com/simonoppowa/OpenNutriTracker](https://github.com/simonoppowa/OpenNutriTracker)：轻松记录您的餐食和零食，并访问庞大的食品及原料数据库，获取详细的营养信息。
    - [ ] ==**好东西**==[https://github.com/zehfernandes/wordnote](https://github.com/zehfernandes/wordnote)：一款简洁优雅的笔记本，用于记录新词汇并探索其含义和同义词。！！！！
        
        ![Untitled](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled.png)
        
- [ ] [paddle支付](https://5km.studio/blog/register-and-verify-paddle-account-in-two-days)
- [ ] [https://x.com/remixdesigner/status/1820359297542525302](https://x.com/remixdesigner/status/1820359297542525302)
- [ ] [https://x.com/remixdesigner/status/1810679992763957724/photo/1](https://x.com/remixdesigner/status/1810679992763957724/photo/1)
- [ ] [https://x.com/ui8/status/1823728492724572444](https://x.com/ui8/status/1823728492724572444)，参考他的 bar
    - 图片
        
        ![image 3](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/image%203.png)
        
- [ ] ph3-mini，手机端运行 [https://x.com/ZHO_ZHO_ZHO/status/1782784109053714915](https://x.com/ZHO_ZHO_ZHO/status/1782784109053714915)

  

---

  

**应用程序简介：**

“GoalMate”。这是一款专为高效目标管理设计的先进AI助手，旨在帮助您轻松实现梦想。

通过GoalMate，您可以清晰地表达您的目标。我们的智能秘书将为您分析并细分目标步骤，确保您不再迷失方向。此外，您可以方便地将当天的活动信息发送给GoalMate，无论是图片、文字还是语音，AI秘书都会精准记录。

更重要的是，GoalMate将根据您的历史记录，为您提供个性化的活动建议，帮助您更有效地规划每一天。不论是日常任务还是长期计划，GoalMate将成为您可靠的伙伴，让您在追逐目标的路上事半功倍。

立即下载GoalMate，让我们一起迈向成功的每一步！

# O

![Untitled 1](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%201.png)

  

  

  

# feature

1. 拍照片，先记录，然后根据你的计划给你分析

  

  

  

定位更改为私人助理

可以上传一些健康类的书籍，也可以走通用的帮助

# UI lib

- [https://wix.github.io/react-native-ui-lib/](https://wix.github.io/react-native-ui-lib/)
- 参考这个的设计做：[https://tamagui.dev/bento#forms](https://tamagui.dev/bento#forms)
- [https://rnr-docs.vercel.app/getting-started/introduction/](https://rnr-docs.vercel.app/getting-started/introduction/)
- [https://twitter.com/shadcn/status/1794655981164720512](https://twitter.com/shadcn/status/1794655981164720512)
- shadcn-ui example [https://github.com/shadcn-ui/ui/blob/06cc0cdf3d080555d26abbe6639f2d7f6341ec73/apps/www/app/(app)/examples/layout.tsx](https://github.com/shadcn-ui/ui/blob/06cc0cdf3d080555d26abbe6639f2d7f6341ec73/apps/www/app/(app)/examples/layout.tsx)
- shadcn-rn 不确定能不能用 [https://github.com/roninoss/rn-primitives](https://github.com/roninoss/rn-primitives)
- 用这个[https://ui.aceternity.com/components/hero-highlight](https://ui.aceternity.com/components/hero-highlight)，参考 frame 的布局，做一个
- 参考一下其他的app出一下产品方案和交互方案: moimoi miley 国外的me

---

Ui

Tab

参考moimoi ，大卡片，每个卡片是个对话，封面是总结的信息和任务，

中间是添加，最右边是信息设置，右上角是账号设置

  

  

# 技术储备

1. GraphRAG 非常适用于 Agnet，创建知识图谱给到全量化精准结果，无需担心切片问题！ [https://x.com/Cydiar404/status/1810328973492314237](https://x.com/Cydiar404/status/1810328973492314237)
2. [https://www.aixinzhijie.com/article/6846242](https://www.aixinzhijie.com/article/6846242)
3. mem0
    
    https://github.com/mem0ai/mem0
    
4. [Groq](https://groq.com/) 速度太快了：Llama-3.1-8b-Instant
5. [GitHub - lobehub/lobe-tts: 🎤 Lobe TTS - A high-quality & reliable TTS/STT library for Server and Browser](https://github.com/lobehub/lobe-tts?tab=readme-ov-file)
6. [GitHub - lobehub/lobe-vidol: 🧸 Lobe Vidol - Making Virtual Idols Accessible for EveryOne](https://github.com/lobehub/lobe-vidol)
7. [Icon Kitchen | Indie Hackers Site - Discover Top Products for Efficient Indie Hacking](https://www.indiehackers.site/en/product/icon-kitchen)
8. [LobeChat 知识库上线 —— 此刻起，跬步千里 · LobeHub](https://lobehub.com/zh/blog/knowledge-base)

---

[https://github.com/AmanVarshney01/expo-tamagui-starter](https://github.com/AmanVarshney01/expo-tamagui-starter)

  

—

# 后端

## supabase

[https://icebreaker.top/articles/2023/5/30-supabase-self-hosting-0/](https://icebreaker.top/articles/2023/5/30-supabase-self-hosting-0/)

[https://github.com/Wsgamer7/blog/blob/main/data/blog/2024/supabase自部署踩坑.mdx](https://github.com/Wsgamer7/blog/blob/main/data/blog/2024/supabase%E8%87%AA%E9%83%A8%E7%BD%B2%E8%B8%A9%E5%9D%91.mdx)

sealos

![Untitled 2](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%202.png)

## db

[https://prisma.dev.org.tw/docs/orm/prisma-client/deployment/edge/deploy-to-cloudflare#postgresql-traditional](https://prisma.dev.org.tw/docs/orm/prisma-client/deployment/edge/deploy-to-cloudflare#postgresql-traditional)

![Untitled 3](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%203.png)

- _创建 HNSW 索引以加速向量搜索_
- 向量数据库和用户数据库分开存储
- graphrag： [https://x.com/llama_index/status/1796936357966954564](https://x.com/llama_index/status/1796936357966954564)
- [https://ollama.com/](https://ollama.com/) ollama 去调用 graphrag ?

  

# comp

input

![Untitled 4](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%204.png)

layout

![Untitled 5](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%205.png)

![Untitled 6](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%206.png)

  

—

[https://tamagui.dev/bento/elements/list#ChatList](https://tamagui.dev/bento/elements/list#ChatList)

![Untitled 7](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%207.png)

  

[https://tamagui.dev/bento/elements/datepickers#DatePicker](https://tamagui.dev/bento/elements/datepickers#DatePicker)

![Untitled 8](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%208.png)

[https://tamagui.dev/bento/user/preferences#LocationNotification](https://tamagui.dev/bento/user/preferences#LocationNotification)

![Untitled 9](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled%209.png)


# old

> 亲切、有趣，强调辅助和私密性。

1. apple 健康
2. 每日提供拍照
3. hi water

—

1. 健身助手
2. 养生助手
    1. 天气
    2. 季节
    3. Action btn

## 资料

[Docus - AI-Powered Health Platform](https://docus.ai/?utm_medium=email&_hsmi=290158984&_hsenc=p2ANqtz-8UC6CoYrGihz5SsWDvAquNHWqw0kBCyshEDB-oeoaQigdhHTl1VKw7gfpT5K8_Ky5J5RDM3T8nx9ZCbpaSYy5JyX6Z_g&utm_content=290158982&utm_source=hs_email)

[AGI新纪元：微软JARVIS与Auto-GPT揭秘，未来智能之门已开 | 回到Axton](https://www.youtube.com/watch?v=-zNSMGScT-U)

激活码为DC3B0B03-8C844F05-BD8CACC1-0E8E2C6C

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81ea9bc1-b02b-403f-942c-4ea40cb5bf50/22363d41-68f1-4b25-bee8-deba0e334dbc/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/81ea9bc1-b02b-403f-942c-4ea40cb5bf50/37926646-e100-4a23-add3-d1e5a2cf465f/Untitled.png)

**sleepAnalysis**

```jsx
[
  {
    "categoryType": "HKCategoryTypeIdentifierSleepAnalysis",
    "device": null,
    "endDate": "2023-12-25T23:25:00.000Z",
    "metadata": {
      "HKWasUserEntered": 1
    },
    "sourceRevision": {
      "operatingSystemVersion": "17.2.0",
      "productType": "iPhone15,4",
      "source": {},
      "version": "17.2"
    },
    "startDate": "2023-12-25T18:25:00.000Z",
    "uuid": "91D94FD5-36FC-4C78-8140-1E6D2233AA9F",
    "value": 0
  },
  {
    "categoryType": "HKCategoryTypeIdentifierSleepAnalysis",
    "device": null,
    "endDate": "2023-12-25T18:25:00.000Z",
    "metadata": {
      "HKWasUserEntered": 1
    },
    "sourceRevision": {
      "operatingSystemVersion": "17.2.0",
      "productType": "iPhone15,4",
      "source": {},
      "version": "17.2"
    },
    "startDate": "2023-12-25T18:25:00.000Z",
    "uuid": "C7C64725-9688-4015-8B07-ECB18283AC80",
    "value": 0
  },
  {
    "categoryType": "HKCategoryTypeIdentifierSleepAnalysis",
    "device": null,
    "endDate": "2023-12-24T18:30:00.000Z",
    "metadata": {
      "HKWasUserEntered": 1
    },
    "sourceRevision": {
      "operatingSystemVersion": "17.2.0",
      "productType": "iPhone15,4",
      "source": {},
      "version": "17.2"
    },
    "startDate": "2023-12-23T18:30:00.000Z",
    "uuid": "5E6347E3-D394-4825-BF14-8E868B3F55D4",
    "value": 1
  },
  {
    "categoryType": "HKCategoryTypeIdentifierSleepAnalysis",
    "device": null,
    "endDate": "2023-12-23T18:59:00.000Z",
    "metadata": {
      "HKWasUserEntered": 1
    },
    "sourceRevision": {
      "operatingSystemVersion": "17.2.0",
      "productType": "iPhone15,4",
      "source": {},
      "version": "17.2"
    },
    "startDate": "2023-12-23T16:59:00.000Z",
    "uuid": "66D43078-F86C-45BF-871A-420BE03AF874",
    "value": 1
  }
]
```