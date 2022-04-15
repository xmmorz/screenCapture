# 本文主要介绍在线屏幕录制 Demo
Its sole method is MediaDevices.getDisplayMedia()
 
!移动端暂不支持

## 环境要求

- 新版本 Chrome,Edge,Firefox 桌面浏览器

## 常见问题

### 1. navigator.mediaDevices为undefined
在不安全的情况下，navigator.mediaDevices是undefined，安全上下文是使用 HTTPS 或file:///URL 方案加载的页面，或者从 localhost.
(https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/getUserMedia)

操作：
 1. 地址为localhost:// 访问时
 2. 地址为https:// 时
 3. 为文件访问file:///
