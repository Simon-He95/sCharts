<p align="center">
<img  src="./assets/icon.jpg" alt="s-charts">
</p>
<p align="center"><a href="https://www.npmjs.com/package/@simon_he/s-charts"><img src="https://img.shields.io/npm/v/@simon_he/s-charts?color=3fb883&amp;label=" alt="NPM version"></a></p>
<p align="center"><a href="https://www.hejian.club/posts/toolsfunction-zh">Docs</a></p>
<p align="center">English | <a href="./README.md">简体中文</a></p>

## sCharts
- Simplify the use of echarts
- It can make your code more concise and beautiful
- Automatically listens for resize events and automatically updates the size of the canvas
- params:
  - container: string | HTMLElement  /* Parent container */
  - options: SChartsOption  /* With echarts options, w: initialization width, h: initialization height, theme: echarts subject, all event behaviors starting with on are called */
  - autoResize: boolean  /* Whether to adjust the width and height automatically */
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
