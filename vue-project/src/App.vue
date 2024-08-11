<script>
import Header from "./components/Header.vue"
import SiteBar from "./components/SiteBar.vue"
import card from "./components/card.vue"



export default{
  components:{Header,SiteBar,card},
  data(){
    return{listCard:[1,2,3,4,5,6,7,8,9,10,11,12]}
  }
}

</script>

<template>
  <div class="wrapper">
    <Header class="header"/>
    <SiteBar class="sitebar" />

    <div class="content">
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
        <card/>
    </div>




  </div>
 
</template>

<style scoped>
.wrapper{
display: grid;
grid-template-columns: 280px 1fr;
grid-template-rows: 72px 95vh;
gap: 36px;
}
.header{grid-area: 1/1/1/3;}
.sitebar{grid-area: 2/1/3/2;}
.content{
  display: flex;
  gap: 24px;
  flex-wrap: wrap;
  grid-area: 2/2/3/3;}

</style>
