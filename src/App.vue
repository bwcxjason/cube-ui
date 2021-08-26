<template>
  <div id="app">
    <div class="radio">
      <cube-radio-group v-model="gaoFengXGW" :options="gaoFengXGWOpts"/>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      gaoFengXGW: 1,	  //岗位
      gaoFengXGWOpts: [
        {
          label: '医疗机构内的发热门诊、隔离病房、新冠核酸检验等存在高风险暴露的医护人员',
          value: 1
        },
        {
          label: '从事呼吸道标本采集和检测的工作人员',
          value: 2
        },
        {
          label: '国际交通运输工具从业人员',
          value: 3
        },
        {
          label: '船舶引航员等登临外籍船舶作业人员',
          value: 4
        },
        {
          label: '移民、海关以及市场监管系统一线工作人员',
          value: 5
        },
        {
          label: '进口冷链食品（含外包装）监管和从业人员',
          value: 6
        },
        {
          label: '口岸进口货物直接接触人员',
          value: 7
        },
        {
          label: '集中隔离医学观察场所工作人员',
          value: 8
        },
        {
          label: '接驳转运工作人员',
          value: 9
        },
        {
          label: '“快捷通道”工作人员',
          value: 10
        },
        {
          label: '其他经风险研判确定的高风险岗位人员',
          value: 11
        },
        {
          label: '均无',
          value: 99,
        }]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  width: 100%;
  font-size: 10px;
}
</style>
