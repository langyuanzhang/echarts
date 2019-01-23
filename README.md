# echarts
使用echarts绘制统计图表

```js
<!--百度图表 ECharts-->
<script src="__common__/js/echarts.js"></script>
<script src="__common__/js/wonderland.js"></script>  <!--主题-->
```

```html
<div class="row" id="main" style="height:600px;background: #ffffff"></div>
```

```js
<script type="text/javascript">
// 基于准备好的dom，初始化echarts实例
var myChart = echarts.init(document.getElementById('main'), 'wonderland');

// 指定图表的配置项和数据
var option = {
    title: {
    text: '用户统计'
    },
    tooltip: {},
    legend: {
    data: ['人']
    },
    xAxis: {
    data: ["1月", "2月", "3月", "4月", "5月", "6月", "7月", "8月", "9月", "10月", "11月", "12月"]
    },
    yAxis: {},
    series: [{
    name: '人数',
    type: 'bar',
    data: [{$jf}]
    }]
};

// 使用刚指定的配置项和数据显示图表。
myChart.setOption(option);

</script>
```