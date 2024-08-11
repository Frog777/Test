<template>

<div class="Card">

<div class="image">
    <div class="hit"><p>Хит продаж</p> <img src="../static/fire.png" alt="fire"> </div>
    <div class="box"><img src="../static/box.png" alt="fire"></div>
    <div class="sale"><p>25%</p></div>
</div>


<div class="desc">
    <h3 class="desc_title">Бренд</h3>
    <p class="desc_text">Полное название товара в несколько строк для вида с обрывом в конце...</p>

    <div class="price">
        <p class="price_act">5990</p>
        <p class="price_old">5990</p>
    </div>

    <button class="btn"><p>Купить</p></button>
</div>


</div>

</template>
<style scoped>
.btn{
    width: 75px;
    height: 38px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 12px 16px 12px 16px;
    border: 1px solid rgb(115, 175, 244);
    border-radius: 8px;
    transition: 0.5s;
    background-color: white;
    cursor: pointer;
}
.btn p{
    color: rgb(115, 151, 245);
    font-size: 14px;
    font-weight: 700;
    line-height: 14px;
    letter-spacing: 0%;
    text-align: left;
}

.price{
    display: flex;
    justify-content: flex-start;
    gap: 8px;
    margin-bottom: 16px;

}
.price_act{
    color: rgb(51, 51, 51);
    font-size: 16px;
    font-weight: 700;
    line-height: 14px;
    letter-spacing: 0%;
    text-align: left;
}
.price_old{
    color: rgb(170, 170, 170);
    font-size: 12px;
    font-weight: 400;
    line-height: 14px;
    letter-spacing: 0%;
    text-align: left;
    text-decoration-line: line-through;
}
.Card{
    width: 333px;
    height: 356px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    padding: 0px;
}
.Card:hover{
    box-shadow: 0px 5px 10px 2px rgba(34, 60, 80, 0.2);
}
.image{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    background:rgb(248, 248, 250);
    width: 100%;
    height: 200px;
    padding: 12px;
}
.box{
    align-self: center;
    flex-grow: 1;
}
.box:hover{
    transform: scale(1.2);
}
.hit{
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: white;
    border-radius: 5px;
    padding: 8px;
    box-shadow: 0px 5px 10px 2px rgba(34, 60, 80, 0.2);
    margin-bottom: 26px;
}
.sale{
    color: rgb(255, 255, 255);
    font-size: 14px;
    font-weight: 700;
    line-height: 14px;
    letter-spacing: 0%;
    text-align: right;
    border-radius: 5px;
    background-color: #7397F5;
    padding: 10px;
}
.desc_title{
    color: rgb(170, 170, 170);
    font-size: 14px;
    font-weight: 400;
    line-height: 16px;
    letter-spacing: 0%;
    text-align: left;
}
</style>