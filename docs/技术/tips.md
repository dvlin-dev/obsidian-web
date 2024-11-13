### 快速跑测试代码

1. vim ~/.zshrc

```jsx
# alias
alias cdtmp='dir=$(mktemp -d /tmp/bowling-XXXXXX) && cd "$dir"'
alias ,r='bunx esno'
```

1. source ~/.zshrc
2. npm install -g bun (如果你没装 bun 的话）
3. cdtmp && vim index.ts 随便写点内容
4. ,r index.ts

> 好处：1. 创建的是临时目录，关机就没了；2. bunx is 100 times faster than npx

### 如何 Profile Node 应用？

1. 跑 Node 时加 `--cpu-prof` 参数，比如 `node --cpu-prof $(which npm) run version`，结束后会产出一个或多个 `.cpuprofile` 文件，
2. 打开 **[https://www.speedscope.app/**](https://www.speedscope.app/**) 上传文件即可查看火焰图，包含详细的堆栈信息。

### 如何找前端咨询

一个 Twitter 搜索技巧，在列表的基础上加各种 filter，包括最低 fav 数、时间、是否包含链接等，比如大家搜 `list:1462723878950690817 since:2023-03-29 min_faves:200 filter:links`，即可包含近期所有的前端资讯。

### Benchmark

• Benchmark 方法，用 brew 装个 hyperfine，然后 `hyperfine --runs 10 'npm -v'` 就可以看到 npm -v 跑 10 次的性能结果。

---

### Mid Jounery 生成 3D 头像

先传自己的照片上去，然后基于此加 prompt「simple avatar, pixar, 3d rendering, flat blue gradient background --s 500 --v 5」，接着就是体力活了，多生成一些，比如 100 个，总能挑到有点像的。

### apple 礼品卡

**Pockyt**