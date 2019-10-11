# AMR.js

播放amr格式的音频文件


### 使用方式

```
 fetch(url)
  .then(response => response.blob())
  .then(blob => AMR.blobToWavUrl(blob))
  .then(url => {
    let audioEl = document.createElement('audio')
    audioEl.preload = 'auto'
    audioEl.src = url
  })
```