# milk-dragon
>>>>>>> 4f693614343a0d3df15667624efdbb545eb1a13f
# 🎄 Grand Luxury Tree - 手势控制的3D圣诞树

哈喽！这是一个为了庆祝圣诞节写的小项目。✨

原本只是想画一棵普通的 3D 圣诞树，但觉得不够酷，于是加上了 **手势识别** 和 **粒子特效**。现在你可以通过摄像头"隔空"控制这棵树，还能把自己喜欢的照片挂上去。

虽然只有几百行代码，但视觉效果拉满了（特别是在大屏幕上）。

<img width="2559" height="1439" alt="image" src="https://github.com/user-attachments/assets/45f3ec57-00b5-4989-b3b2-484772ad95cf" />

## ✨ 最新更新

- 🚀 **优化加载性能** - 大幅减少启动时间
- 📁 **配置文件驱动** - 照片管理更简单，支持本地路径
- 🖼️ **本地照片支持** - 无需上传，直接配置本地图片路径
- 🎯 **更好的错误处理** - 加载失败时的优雅降级

## 🤔 这是啥？(Intro)

这不是那种静态的网页贺卡。这是一棵由 **几千个粒子** 组成的动态树。
我接入了 Google 的 MediaPipe，所以它能看懂你的手势。

* **粒子特效**：树会呼吸、旋转，还能炸裂成满天星。
* **隔空控物**：不需要鼠标，对着摄像头挥挥手就能控制它（感觉像奇异博士）。
* **配置化照片**：通过 `images.json` 配置照片，支持本地路径和网络图片。
* **极简审美**：只有黑金配色，没有花里胡哨的装饰，主打一个"高级感"。

<img width="2557" height="1291" alt="image" src="https://github.com/user-attachments/assets/d7d31b4c-bf4d-49b2-b922-79813bbddba5" />

## 🛠️ 用了什么 (Tech)

纯纯的前端魔法，没用复杂的框架：
* **Three.js** - 搞定 3D 渲染和粒子系统。
* **MediaPipe** - 搞定手势识别（这东西太强了）。
* **原生 JS (ES Modules)** - 手搓核心逻辑。

## 🎮 怎么玩？(Controls)

### 🖐️ 手势模式 (重点！)
确保浏览器允许使用摄像头，然后：
1.  **张开手掌 (🖐️)**：这就是"炸裂模式"！树会散开变成星云，你可以转动视角。
2.  **握紧拳头 (✊)**：收！粒子会重新聚合成圣诞树。
3.  **捏合手指 (🤏)**：就像在捏东西一样，它会随机抓取一张照片放大给你看。

### 🖱️ 鼠标党
* 左键拖拽旋转，滚轮缩放。
* **H 键**：按下可以隐藏所有 UI，用来截图或录屏当壁纸很棒。

## 📸 照片配置

### 添加你的照片
1. 将照片复制到 `./images/` 文件夹
2. 编辑 `images.json` 配置文件：

```json
{
  "photos": [
    {
      "path": "./images/my-photo.jpg",
      "title": "我的照片",
      "description": "照片描述"
    }
  ]
}
```

### 支持的路径格式
- 本地路径：`./images/photo.jpg`
- 子文件夹：`./images/family/christmas.png`
- 网络图片：`https://example.com/image.jpg`

## 🚀 跑起来 (How to Run)

⚠️ **注意：** 因为用到了 ES Modules 和摄像头权限，**千万不要直接双击 HTML 文件打开**，浏览器会报错（CORS 策略限制）。你得起一个本地服务器。

**推荐方式：**
```bash
# Python
python -m http.server 8000

# Node.js
npx http-server .

# VS Code
# 安装 Live Server 插件，右键 HTML 文件选择 "Open with Live Server"
```

然后浏览器访问 `localhost:8000/chistmas_tree_final.html`。

## 📁 项目结构

```
├── chistmas_tree_final.html  # 主页面
├── images.json               # 照片配置文件
├── images/                   # 本地照片文件夹
│   ├── sample1.jpg          # 示例照片
│   ├── sample2.jpg          # 示例照片
│   └── README.md            # 照片使用说明
└── README.md                # 项目说明
```

**Merry Christmas! 🎅**
如果你觉得这项目有点意思，欢迎 Star，或者 Fork 改成你喜欢的颜色！
=======
# milk-dragon
>>>>>>> 4f693614343a0d3df15667624efdbb545eb1a13f
