# 贪食蛇游戏 🐍

一个使用原生 JavaScript 开发的经典贪食蛇网页游戏，具有流畅的动画效果和现代化的界面设计。

## 在线演示

[点击这里体验游戏](https://xiaoo666.github.io/SnakeGame/) <!-- 部署到 GitHub Pages 后此链接将生效 -->

## 功能特点

- 🎮 **流畅的游戏体验** - 基于 Canvas 的高性能渲染
- 🎨 **现代化界面** - 渐变色设计和发光特效
- 📊 **分数系统** - 实时分数显示和最高分记录
- 💾 **本地存储** - 自动保存历史最高分
- ⏸️ **游戏控制** - 支持开始、暂停、重新开始
- 🎯 **碰撞检测** - 精确的墙壁和自身碰撞判定
- 🎚️ **难度选择** - 简单、普通、困难三种难度等级
- 📱 **响应式设计** - 适配不同屏幕尺寸

## 技术栈

- **HTML5** - 页面结构
- **CSS3** - 样式和动画效果
- **JavaScript (ES6)** - 游戏逻辑
- **Canvas API** - 图形渲染

## 快速开始

### 方法一：直接打开

1. 克隆或下载本仓库
```bash
git clone https://github.com/xiaoo666/SnakeGame.git
```

2. 在浏览器中打开 `index.html` 文件即可开始游戏

### 方法二：本地服务器

使用本地服务器运行（推荐）：

```bash
# 使用 Python 3
python -m http.server 8000

# 使用 Python 2
python -m SimpleHTTPServer 8000

# 使用 Node.js (需要安装 http-server)
npx http-server
```

然后在浏览器访问 `http://localhost:8000`

## 游戏玩法

### 控制方式

- **↑** - 向上移动
- **↓** - 向下移动
- **←** - 向左移动
- **→** - 向右移动

### 游戏规则

1. 使用方向键控制贪食蛇的移动方向
2. 吃到红色食物可以增加 10 分，同时蛇身变长
3. 撞到墙壁或自己的身体会导致游戏结束
4. 尽可能获得更高的分数！

### 难度等级

- **简单** - 蛇移动速度较慢（150ms），适合新手
- **普通** - 蛇移动速度中等（100ms），标准难度
- **困难** - 蛇移动速度较快（60ms），挑战高分

### 操作按钮

- **难度选择** - 在游戏开始前选择难度（简单/普通/困难）
- **开始游戏** - 启动新游戏
- **暂停** - 暂停/继续游戏
- **重新开始** - 重置游戏状态

## 项目结构

```
SnakeGame/
│
├── index.html          # 主HTML文件
├── style.css           # 样式文件
├── game.js             # 游戏逻辑
└── README.md           # 项目说明文档
```

## 代码说明

### 核心功能模块

- **游戏初始化** (`initGame`) - 重置游戏状态
- **蛇的移动** (`moveSnake`) - 处理蛇的移动逻辑
- **碰撞检测** (`checkCollision`) - 检测墙壁和自身碰撞
- **食物生成** (`generateFood`) - 随机生成食物位置
- **游戏渲染** (`drawGame`) - Canvas 绘制游戏画面
- **分数管理** (`updateScore`) - 更新和保存分数

### 关键参数

```javascript
const GRID_SIZE = 20;        // 网格大小
const TILE_COUNT = 20;       // 网格数量

// 难度等级对应的速度
const DIFFICULTY_SPEEDS = {
    easy: 150,      // 简单：150ms
    normal: 100,    // 普通：100ms
    hard: 60        // 困难：60ms
};
```

## 开发计划

- [x] 添加难度选择（速度调节）
- [ ] 添加音效和背景音乐
- [ ] 增加特殊道具系统
- [ ] 添加排行榜功能
- [ ] 支持移动端触摸控制
- [ ] 添加主题切换功能
- [ ] 多语言支持

## 浏览器兼容性

- ✅ Chrome (推荐)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Opera

## 贡献

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的改动 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

## 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情

## 作者

xiaoo666 - [@xiaoo666](https://github.com/xiaoo666)

项目链接: [https://github.com/xiaoo666/SnakeGame](https://github.com/xiaoo666/SnakeGame)

## 致谢

- 灵感来源于经典的贪食蛇游戏
- 感谢所有贡献者的支持

---

⭐️ 如果这个项目对你有帮助，请给个 Star 吧！
