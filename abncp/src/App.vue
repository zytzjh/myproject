<template>
  <div id="app">
    <router-view/>
    <Lefttop></Lefttop>
  </div>
</template>

<script>
	//引入Lefttop组件
import Lefttop from '@/components/Lefttop'


export default {
  name: 'App',
  components:{
    Lefttop
  }

}

</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;  
}
</style>
