<template>
  <div class="content-box">
    <div> <base-table :columns="columns" needRadio="true"></base-table></div>
    <div> <base-table :columns="columns1"></base-table></div>
  </div>
</template>

<script>
import baseTable from '../../../components/components-element-ui/base-table.vue'
export default{
  components:{baseTable},
  name: 'index',
  data () {
    return {
      columns:[
        {
           prop:'name',  //英文字段名称
           label:'名字', //中文字段名称
           width:'180',

        },
        {
           prop:'sex',
           label:'性别',
           width:'180',
        },
        {
           prop:'address',
           label:'地区',
           width:'180',
        },
        {
           prop:'hobby',
           label:'爱好',
           width:'180',
        },
        {
           prop:'date',
           label:'日期',
           width:'180',
        },
      ],
        columns1: [
        {
          prop: 'name',  //英文字段名称
          label: '名字', //中文字段名称
          width: '180',
        },
        {
          prop: 'sex',
          label: '性别',
          width: '180',
        },
        {
          prop: 'address',
          label: '地区',
          width: '180',
        },
        {
          prop: 'hobby',
          label: '爱好',
          width: '180',
        },
        {
          prop: 'date',
          label: '日期',
          width: '180',
        },
      ]
    }
  },
  created () {},
  mounted () {},
  methods: {}
}
</script>

<style scoped lang="scss">
.content-box > div{
  margin-top:30px
}
</style>
