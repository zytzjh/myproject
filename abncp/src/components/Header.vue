<template>
  <div class="header">
    <div class="head-left">
      <h3 class="head">{{ head }}</h3>
      
      <el-dropdown trigger="click">
          <span class="el-dropdown-link">
          决策指挥系统<i class="el-icon-arrow-down el-icon--right"></i>
           </span>
           <el-dropdown-menu slot="dropdown">
           <el-dropdown-item command="a">黄金糕</el-dropdown-item>
           <el-dropdown-item command="b">狮子头</el-dropdown-item>
           <el-dropdown-item command="c">螺蛳粉</el-dropdown-item>
           <el-dropdown-item command="d">双皮奶</el-dropdown-item>
           <el-dropdown-item command="e" divided>蚵仔煎</el-dropdown-item>
           </el-dropdown-menu>
     </el-dropdown>

    </div>

    



    <div class="head-right">
        <img class="portrait" src="../assets/logo.png" alt="">
        <span class="name">{{ name }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  methods: {
    handleCommand(command) {
      this.$message("click on item " + command);
    }
  },
  data() {
    return {
      head: "四川省防讯抗旱调度决策指挥平台",
      name: "张松青"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  width: 100;
  height: 40px;
  line-height: 40px;
  background-color: #7cbefc;
  padding-left: 10px;
  padding-right: 10px;
}
.head-left {
  float: left;
}
.head-right {
  float: right;
  border-left: 1px solid red;
  width: 90px;
  height: 40px;
  line-height: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.portrait {
  width: 20px;
  height: 20px;
}
.name {
  font-size: 12px;
  padding-left: 10px;
}

.head {
  display: inline;
}
.policy {
  margin-left: 10px;
}


.el-dropdown-link {
  cursor: pointer;
  color: white;
  font-size: 14px;
  font-weight: 600;
  padding-left: 10px;
}
.el-icon-arrow-down {
  font-size: 12px;
}
</style>
