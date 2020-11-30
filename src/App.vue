<template>
  <div id = "app">
      <!-- <button @click="to">到</button> -->
      <router-view></router-view>
  </div>
</template>

<script>
import AsideNav from "./components/AsideNav"
export default {
  
  methods :{
    // to(){
    //   this.$router.push({
    //     path : "/news"
    //   })
    // }
  }
}
</script>

<style>
  body,h1,h2,h3,h4,h5,h6,p,ul,ol,dl,dd,hr,ul,ol,td,input,option,textarea{
	margin:0;
	padding:0;
}
body{
	font-family: "微软雅黑";
}
li{
	list-style: none;
}
a{
	text-decoration: none;
}
img{
	border: none;
}
#app{
  width: 100%;
}
</style>