## * 案例：悦听播放器

[网易云音乐API接口服务](https://autumnfish.cn/)

1. 实现最终效果演示

2. 实现步骤分析

   > 获取搜索歌曲：<https://autumnfish.cn/search?keywords=星月神话>
   >
   > 获取当前歌曲： <https://autumnfish.cn/song/url?id=33894312> 
   >
   > 歌曲封面获取：<https://autumnfish.cn/song/detail?ids=347234> 
   >
   > 获取歌曲评论：<https://autumnfish.cn/comment/hot?type=0&id=186015> 

   1. 顶部搜索歌曲输入框 v-model = "keyword"
   2. 点击回车 @keyup.enter="searchMusic" 
   3. 点击放大镜 @click="searchMusic" 
   4. searchMusic这个方法里面发送 axios  get请求
   5. 返回回来歌曲列表的数据 musicList 保存歌曲列表
   6. 将歌曲列表数据musicList 使用v-for渲染到页面上去
   7. 双击要播放的歌曲 @dblclick="playMusic"
   8. playMusic这个方法我们还要请求封面数据，还要有播放的效果
   9. 点击暂停或者播放 @pause @play 执行播放或者暂停的效果

3. 代码结构演示

4. 开发过程演示

5. 所用知识及注意事项小结

   > 版权问题，企业中，如果要做播放器，一定要考虑版权问题，学习节点，个人玩耍，只要不商用，不盈利，不会涉及侵权

