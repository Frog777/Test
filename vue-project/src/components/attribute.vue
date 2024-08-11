<template>
<div class="attribute">
<input type="checkbox" value="1" >
<p class="val">Атрибут</p>
<p>3</p>
</div>


</template>

<style scoped>
input,input:hover{
    border: 1px solid rgb(115, 151, 245);
    border-radius: 3px;
    width: 20px;
    height: 20px;
    outline: none;
}
.attribute{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 16px 0 0;

}
.val{
    flex-grow: 1;
    margin: 0;
}


</style>