<template>
  <div>
    <Chart :cdata="cdata" />
  </div>
</template>

<script>
import Chart from './chart.vue';
export default {
  data () {
    return {
      cdata: [
        {
          // 地图中的数据位于chart.vue 中，为各个省市的坐标
          name: '福州市',
          value: 10,
          elseData:{
            // 这里放置地图 tooltip 里想显示的数据
            name: 'aaaaaaaa',
            value: 8
          }
        },
        {
          name: '厦门市',
          value: 9,
        },
        {
          name: '漳州市',
          value: 8,
        },
        {
          name: '泉州市',
          value: 7,
        },
        {
          name: '三明市',
          value: 6,
        },
        {
          name: '莆田市',
          value: 5,
        },
        {
          name: '南平市',
          value: 4,
        },
        {
          name: '龙岩市',
          value: 3,
        },
        {
          name: '宁德市',
          value: 2,
        }
      ]
    }
  },
  components: {
    Chart,
  },
  mounted () {
  },
  methods: {
  }
}
</script>

<style lang="scss" scoped>
</style>
