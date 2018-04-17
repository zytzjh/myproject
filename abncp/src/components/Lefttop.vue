<template>
  <div class="lefttop">
      <div class="lefttop-one">
              
              <div class="lefttop-oneleft">
                  <div class="lefttop-oneoka"></div>
                  <div class="lefttop-oneokb">我的关注</div>
              </div>
              <div class="lefttop-oneright"><a href="#"><i class="iconfont icon-zhankai"></i></a></div>
      </div>
      <div class="lefttop-two">

<el-row class="tac">         
<el-menu
      default-active="2"
      class="el-menu-vertical-demo"
      @open="handleOpen"
      @close="handleClose"
      >
   
      <el-submenu index="1">
        <template slot="title">
          <i class="el-icon-menu"></i>
          <span>雨晴详情</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">选项1</el-menu-item>
          <el-menu-item index="1-2">选项2</el-menu-item>
          <el-menu-item index="1-3">选项3</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="2">
        <template slot="title">
          <i class="el-icon-menu"></i>
          <span>河道水情</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">选项1</el-menu-item>
          <el-menu-item index="1-2">选项2</el-menu-item>
          <el-menu-item index="1-3">选项3</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
        <el-submenu index="3">
        <template slot="title">
          <i class="el-icon-menu"></i>
          <span>水库</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">选项1</el-menu-item>
          <el-menu-item index="1-2">选项2</el-menu-item>
          <el-menu-item index="1-3">选项3</el-menu-item>
        </el-menu-item-group>
      </el-submenu>

      </el-menu>
</el-row>   


      </div>
  </div>
</template>

<script>
 export default {
  name: 'Lefttop',
  data () {
    return {
      
    }
  }
}
</script>

<style scoped>
    .lefttop{
        width: 340px;
        height: 290px;
        border: 1px solid #000000;
    }
    .lefttop-one{
        width: 100%;
        height: 60px; 
        line-height:60px;
        border-bottom: 4px solid #f6f6f6;
        /* box-shadow: 0px 5px 0px #000000; */
    }
    
    .lefttop-oneleft{
        float:left;
        padding-left: 10px;
        /* border-left: 4px solid red; */
        margin-left:10px;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .lefttop-oneoka{
        float: left;
        width: 5px;
        height: 20px;
        background-color: red;
        margin-right: 20px;
    }
    .lefttop-oneokb{
        float: left;
    }
    .lefttop-oneright{
        float:right;
        padding-right:10px;
    }

    .lefttop-two{
        width: 100%;
        height: 220px;
        overflow:auto;
        background-color: white;
        
    }


</style>
