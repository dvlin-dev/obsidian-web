
> llm最简单的办法，去把 langchain 搞懂，看看每个api都是干什么的，搜索关键词，看源码

> 基于大语言模型构建知识问答系统  
> 传统搜索系统基于关键字匹配，在面向：游戏攻略、技术图谱、知识库等业务场景时，缺少对用户问题理解和答案二次处理能力。本文探索使用大语言模型（Large Language Model, LLM），通过其对自然语言理解和生成的能…  
> [https://zhuanlan.zhihu.com/p/627655485](https://zhuanlan.zhihu.com/p/627655485)  

> LLM+Embedding构建问答系统的局限性及优化方案  
> 近期LangChain + LLM 方案高速发展，降低了知识问答等下游应用的开发门槛。但随着业务深入，一些局限性也日渐显露，比如：LLM意图识别准确性较低，交互链路长导致时间开销大；Embedding 不适合多词条聚合匹配等。…  
> [https://zhuanlan.zhihu.com/p/641132245](https://zhuanlan.zhihu.com/p/641132245)  

> ChatGPT 系列教程 - 提问篇：Prompt 的高级概念  
> 在上一篇文章中，我们发现随着不断改进 Prompt ，你就能从 ChatGPT 中得到更好的响应结果。 说白话就是，“你问题问的越好，你得到的答案也就越好”。 这就是 Prompt 的核心理念，为了满足需求不断优化你的提问。 …  
> [https://zhuanlan.zhihu.com/p/623395924](https://zhuanlan.zhihu.com/p/623395924)  

1. 对问题进行整理，语法纠错、确定问题细节等，引导用户二次询问，然后对问题向量化
    
    1. 学习如何使用 langchain 引导用户，完善该问题
    
    ![Untitled](https://dvlin-notes-assets.oss-cn-beijing.aliyuncs.com/Untitled.png)
    
2. tokenizer 分词器，保证拆分的词是有含义的（[tiktoken](https://link.zhihu.com/?target=https%3A//github.com/openai/tiktoken)
3. 反馈系统：
    
    1. 类似gpt的反馈，赞、中等、差，点击后记录用户上下文发送给后台，继续优化知识库。
    
      
    
      
    

# 需要学习点

- score threshold 过高或 top k 过低