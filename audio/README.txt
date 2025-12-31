# 音频文件使用说明

## 📁 目录说明

本目录用于存放本地音乐文件，项目会从这里加载音频。

## 📥 如何添加音乐文件

### 方法一：从包图网下载
1. 访问 https://ibaotu.com/yinxiao
2. 搜索你需要的音乐类型
3. 登录包图网账号
4. 下载音频文件（mp3 或 wav 格式）
5. 将文件复制到此目录
6. 重命名文件为 song1.mp3, song2.mp3 等

### 方法二：使用自有音频
1. 将你自己的 MP3 文件复制到此目录
2. 重命名文件为 song1.mp3, song2.mp3 等
3. 在 musicData.js 中更新对应的 audioUrl

## 🔧 配置音频路径

在 src/data/musicData.js 文件中，将 audioUrl 修改为本地路径：

```javascript
// 修改前（网络地址）
audioUrl: "https://actions.google.com/sounds/v1/alarms/beep_short.ogg"

// 修改后（本地路径）
audioUrl: "/audio/song1.mp3"
```

## 📋 音频文件命名建议

按照歌曲 ID 命名，方便管理：
- song1.mp3 - 夜空中最亮的星
- song2.mp3 - 晴天
- song3.mp3 - 稻香
- song4.mp3 - 平凡之路
- song5.mp3 - 消愁
- song6.mp3 - 光年之外
- song7.mp3 - 体面
- song8.mp3 - 成都
- song9.mp3 - 青花瓷
- song10.mp3 - 追梦赤子心

## ✅ 示例配置

```javascript
{
  id: 1,
  title: "夜空中最亮的星",
  artist: "逃跑计划",
  album: "世界",
  duration: 265,
  audioUrl: "/audio/song1.mp3",  // 本地路径
  cover: "https://i.scdn.co/image/...",
  category: "流行"
}
```

## 📝 注意事项

1. 确保音频文件格式为 mp3、wav 或 ogg
2. 文件名使用英文，避免中文和特殊字符
3. 音频文件大小建议不超过 10MB
4. 确保音频文件不侵犯版权

## 🎵 推荐免费音乐资源网站

- Free Music Archive: https://freemusicarchive.org
- Jamendo: https://www.jamendo.com
- SoundCloud (需要找免版权音乐)
- Bensound: https://www.bensound.com
- Purple Planet: https://www.purple-planet.com
