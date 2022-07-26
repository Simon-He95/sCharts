<p align="center">
<img  src="./assets/icon.jpg" alt="s-charts">
</p>
<p align="center"><a href="https://www.npmjs.com/package/@simon_he/s-charts"><img src="https://img.shields.io/npm/v/@simon_he/s-charts?color=3fb883&amp;label=" alt="NPM version"></a></p>
<p align="center"><a href="https://www.hejian.club/posts/toolsfunction-zh">Docs</a></p>
<p align="center"> <a href="./README_en.md">English</a> | 简体中文</p>

## sCharts
- 简单化echarts使用
- 可以让你的代码更加简洁,更加美观
- 不需要在onMounted中执行,可以在任意时刻使用
- 自动监听resize事件,自动更新canvas的大小
- 参数:
  - container: string | HTMLElement, 父容器
  - options: SChartsOption, echarts配置options,扩展了w: 初始化宽度, h: 初始化高度, theme: echarts主题, 所有的事件行为以on开头都会被调用
  - autoResize: boolean, 是否自动调整宽高
```javascript
const charts = sCharts('#main', {
  w: 500,
  h: 300,
  theme: 'dark',
  xAxis: {
    data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
  },
  yAxis: {},
  series: [
    {
      type: 'bar',
      data: [23, 24, 18, 25, 27, 28, 25],
    },
  ],
})
```
