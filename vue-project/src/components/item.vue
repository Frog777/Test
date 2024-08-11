<script>
export default{
    data(){
        return{
        }
    },
    props:{val:{type:String}}

};
</script>
<template>
    <div class="categories_item">
        <img class="vector" src="../static/Vector.png" alt="vector">
        <p class="val">{{ val }}</p>
        <p>3</p>
    <slot></slot>
</div>
</template>
<style scoped>

.categories_item{
    display: flex;
    align-items: center;
    padding: 0 16px 0 0
}
.val{
    flex-grow: 1;
}




.vector{width: 9px; height: 16px; margin-right: 7px; align-self: center;}

</style>