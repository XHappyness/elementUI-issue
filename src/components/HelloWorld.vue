<template>
  <div class="home">
    <el-select 
            style="width:100%;" 
            v-model="value10" 
            multiple 
            filterable 
            placeholder="请选择文章标签">
            <el-option v-for="item in options5" :key="item.value" :label="item.label" :value="item.value">
            </el-option>
          </el-select>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      options5 : [{
        value: '1',
        label: '1111111111111111111'
      }, {
        value: '2',
        label: '2222222222222222222'
      }, {
        value: '3',
        label: '333333333333333333'
      },{
        value: '4',
        label: '444444444444444444'
      }, {
        value: '5',
        label: '55555555555555555'
      }, {
        value: '6',
        label: '66666666666666666'
      }],
      value10 : []
    }
  }
}
</script>

<style>
 .home{
            width: 500px;
        }
</style>
