# 🏛️ 山东省智慧旅游数据监控平台

<div align="center">

![Vue](https://img.shields.io/badge/Vue-3.5.13-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5.7.2-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6.1.0-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![ECharts](https://img.shields.io/badge/ECharts-5.6.0-AA344D?style=for-the-badge&logo=apache-echarts&logoColor=white)

**🌊 齐鲁大地，智慧旅游，数据驱动未来**

[在线预览](https://sd-tourism-dashboard-open.vercel.app/) • [项目介绍](#项目介绍) • [功能特色](#功能特色) • [技术栈](#技术栈) • [快速开始](#快速开始)

</div>

---

## 📊 项目介绍

山东省智慧旅游数据监控平台是一个基于 Vue 3 + TypeScript + ECharts 构建的现代化数据可视化项目。平台以山东省旅游数据为核心，通过直观的图表展示、实时数据监控和智能分析，为旅游管理部门提供全面的数据洞察。

### 🎯 核心价值

- **数据可视化**：多维度展示山东省旅游数据
- **实时监控**：动态更新旅游指标和趋势
- **智能分析**：深度挖掘旅游数据价值
- **美观界面**：现代化UI设计，用户体验优秀

---

## ✨ 功能特色

### 🗺️ 地理信息展示

- **山东省地图**：精确的地理边界和行政区划
- **3D柱状图**：各城市旅游数据立体展示
- **动态高亮**：循环高亮显示不同城市数据

### 📈 数据可视化组件

#### 左侧面板

- **游客年龄分布**：3D立方体柱状图，循环高亮效果
- **景点人流排名**：实时滚动排名，进度条可视化
- **年度接待游客比**：双年度对比折线图

#### 右侧面板

- **各行业收入**：渐变柱状图，循环高亮展示
- **实时热词**：散点图展示热门旅游关键词
- **接待游客TOP5**：特殊形状柱状图，数值标签显示

### 🎨 界面特色

- **深色主题**：科技感十足的深色背景
- **动态效果**：流畅的动画和过渡效果
- **响应式设计**：适配不同屏幕尺寸
- **自定义字体**：独特的LED数字字体

---

## 🛠️ 技术栈

| 技术                     | 版本   | 用途        |
| ------------------------ | ------ | ----------- |
| **Vue**                  | 3.5.13 | 前端框架    |
| **TypeScript**           | 5.7.2  | 类型安全    |
| **Vite**                 | 6.1.0  | 构建工具    |
| **ECharts**              | 5.6.0  | 数据可视化  |
| **Sass**                 | 1.89.2 | CSS预处理器 |
| **Vue3-scroll-seamless** | 1.0.6  | 无缝滚动    |

### 🎯 核心技术特性

- **Vue 3 Composition API**：现代化的组件开发方式
- **TypeScript**：完整的类型定义和类型安全
- **ECharts 5**：强大的数据可视化能力
- **自定义图形**：3D立方体、特殊形状等自定义图表
- **动态高亮**：定时器控制的循环高亮效果

---

## 🚀 快速开始

### 环境要求

- Node.js >= 16.0.0
- pnpm >= 7.0.0

### 安装依赖

```bash
# 克隆项目
git clone https://github.com/your-username/shandong-tourism-monitor.git

# 进入项目目录
cd shandong-tourism-monitor

# 安装依赖
pnpm install
```

### 开发运行

```bash
# 启动开发服务器
pnpm dev

# 构建生产版本
pnpm build

# 预览生产版本
pnpm preview
```

### 项目结构

```
山东省智慧旅游数据监控平台/
├── src/
│   ├── components/          # 组件目录
│   │   ├── common/         # 通用组件
│   │   ├── leftPanel/      # 左侧面板组件
│   │   └── rightPanel/     # 右侧面板组件
│   ├── assets/             # 静态资源
│   │   ├── data/          # 数据文件
│   │   └── images/        # 图片资源
│   ├── styles/            # 样式文件
│   └── types/             # 类型定义
├── public/                # 公共资源
└── package.json          # 项目配置
```

---

## 📊 数据展示

### 🏛️ 山东省主要景点

- **泰山**：五岳独尊，世界文化与自然双重遗产
- **曲阜三孔**：儒家文化发源地，世界文化遗产
- **青岛栈桥**：海滨城市标志性建筑
- **蓬莱阁**：人间仙境，八仙过海传说
- **台儿庄古城**：运河文化，抗战纪念地

### 📈 核心数据指标

- **游客接待量**：实时监控各城市游客数据
- **行业收入**：旅游、住宿、餐饮、购物等细分数据
- **年龄分布**：游客年龄结构分析
- **热门景点**：景点人流排名和热度分析

---

## 🎨 设计亮点

### 🎯 视觉设计

- **深色科技风**：符合数据监控平台的视觉定位
- **渐变色彩**：丰富的色彩层次和视觉冲击
- **动态效果**：流畅的动画和交互体验
- **信息层次**：清晰的信息架构和视觉引导

### 🔧 交互体验

- **循环高亮**：自动循环高亮不同数据项
- **无缝滚动**：流畅的列表滚动效果
- **响应式布局**：适配不同设备屏幕
- **实时更新**：动态数据更新和展示

---

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request 来帮助改进这个项目！

### 开发规范

- 使用 TypeScript 进行类型安全开发
- 遵循 Vue 3 Composition API 最佳实践
- 保持代码风格一致，使用 ESLint + Prettier
- 添加适当的注释和文档

### 提交规范

```bash
feat: 添加新功能
fix: 修复bug
docs: 更新文档
style: 代码格式调整
refactor: 代码重构
test: 添加测试
chore: 构建过程或辅助工具的变动
```

---

## 📄 许可证

本项目采用 [MIT License](LICENSE) 开源许可证。

---

## 🙏 致谢

感谢以下开源项目和技术社区的支持：

- [Vue.js](https://vuejs.org/) - 渐进式JavaScript框架
- [ECharts](https://echarts.apache.org/) - 数据可视化图表库
- [Vite](https://vitejs.dev/) - 下一代前端构建工具
- [TypeScript](https://www.typescriptlang.org/) - JavaScript的超集

---

<div align="center">

**🌟 如果这个项目对您有帮助，请给它一个 Star！**

Made with ❤️ in Shandong, China

</div>
