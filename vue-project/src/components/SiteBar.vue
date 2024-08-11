<script>
import item from "../components/item.vue"
import attribute from "../components/attribute.vue"



export default{
  components:{item,attribute},
  data(){
    return{
        categories:['Название категории','Название категории','Название категории',],
        catIndex: 0,
        attribute:[1,2,3,4,5]

    }
  },
  methods:{
    Toggle(index){
       if (this.catIndex!=index){
        this.catIndex=index
       }else{
        this.catIndex=-1
       }
    }
  }
}

</script>

<template>


<div class="siteBar">

<!-- КАТЕГОРИИ  -->

<div class="categories" v-for="(val,index) in categories" :key="index">
  <item @click="Toggle(index)" :val="val"></item>
    <div class="podCat" v-show="catIndex==index">
      <div class="podCat__row"><p>{{ val }}</p><p class="lenght_row">{{ categories.length }}</p></div>
      <div class="podCat__row"><p>{{ val }}</p><p class="lenght_row">{{ categories.length }}</p></div>
      <div class="podCat__row"><p>{{ val }}</p><p class="lenght_row">{{ categories.length }}</p></div>
    </div>
</div>

<!-- ЦЕНА -->

<div class="price">
  <div class="title"><h3>Цена</h3></div>
    <div class="input"><input type="text" placeholder="от"></div>
      <div class="tt"></div>
    <div class="input"><input type="text" placeholder="от"></div>
</div>

<!-- БРЕНД -->



<div class="change">
  <h3 class="brand">Бренд</h3>
  <p class="clear">Очистить</p>
</div>
<div class="change__search">
    <img class="change_img"  src="../static/Frame.png" alt="logo">
    <input type="text" placeholder="Поиск">
</div>

<div class="attribute_list" v-for="(val,index) in attribute" :key="index">
  <attribute/>
</div>

<div class="size">
<h3 class="title">Размер</h3>
  <div class="attribute_list" v-for="(val,index) in attribute" :key="index">
  <attribute/>
  </div>
</div>






</div>

</template>
<style scoped>
.change{
  display: flex;
  justify-content: space-between;
}
.brand{
  color: rgb(51, 51, 51);
  font-size: 16px;
  font-weight: 700;
  line-height: 20px;
  letter-spacing: 0%;
  text-align: left
}
.clear{
  color: rgb(170, 170, 170);
  font-size: 12px;
  font-weight: 400;
  line-height: 12px;
  letter-spacing: 0%;
  text-align: right;
  text-decoration-line: underline;
  align-self: center;
  cursor: pointer;
}
.change__search{
  display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    padding: 4px 16px 4px 16px;
    border: 1px solid rgb(213, 213, 213);
    border-radius: 10px;
    background: rgb(255, 255, 255);
    height: 48px;
}
.change_img{
  width: 16.67px;
  height: 16.67px;
}
.attribute_list{
  display: flex;
  flex-direction: column;

}





.price{
  display: grid;
  grid-template: 1fr 1fr / 1fr 1fr 1fr; 
  width: 280px;
}
.title{
  grid-area: 1/1/1/4;
  display: flex;
  justify-content: center;
  align-items: center;
}
.title p{
  color: rgb(51, 51, 51);
  font-size: 16px;
  font-weight: 700;
  line-height: 20px;
  letter-spacing: 0%;
  text-align: left;
  margin: 0 auto;
}

.input{
  width: 119px;
  display: flex;
  justify-content: center;
  border: 1px solid rgb(213, 213, 213);
  border-radius: 4px;
  padding: 10px 8px;
}
.input input,input:focus{
  width: 117px;
  border: none;
  outline: none;
}
.tt{
  margin: auto 16px;
  width: 10px;
  height: 1px;
  background: rgb(213, 213, 213);
}




.siteBar{
    width: 17.5rem;
    min-height: 47.5rem;
    flex-direction: column;
}
.categories{
    display: flex;
    flex-direction: column;
    cursor: pointer;
}

.items{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}
.podCat{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 0px 16px 0px 32px;
}
.podCat__row{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}


.categories:hover{background-color: #E2EFFF; border-radius: 5px;}

</style>