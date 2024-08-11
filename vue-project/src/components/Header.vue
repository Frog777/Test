<script>

</script>

<template>
<div class="header">
    <div class="header__firstBox">
        <div class="logo">
            <img class="logo__img" src="../static/logo.png" alt="logo">
            <p>Логотип</p>
        </div>

        <button class="btn">Каталог</button>
    
    </div>



<div class="header__search">
    <img src="../static/Frame.png" alt="logo">
    <input type="text" placeholder="Поиск по 100 000 товаров ">
</div>

<div class="header__nav" >
    <ul class="nav__list">
        <li>Информация о компании</li>
        <li>Контакты</li>
        <li>Полезные ссылки</li>
    </ul>
</div>



</div>
</template>

<style scoped>
.header{
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    padding: 12px 0px 12px 0px;
}

.header__firstBox{
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 24px;
}
.logo{
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 12px 24px;
    gap: 8px;

}
.logo img{
    width: 24px;
    height: 24px;
}

.btn{
    width: 104px;
    height: 48px;
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    padding: 8px 24px 8px 24px;
    box-sizing: border-box;
    border: 1px solid rgb(115, 175, 244);
    border-radius: 8px;
    transition: 0.5s;
}
.btn:hover{
    transform: scale(1.1);
}


.header__search{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 4px 16px 4px 16px;
    border: 1px solid rgb(115, 175, 244);
    border-radius: 10px;
    background: rgb(255, 255, 255);
    width: 1015px;
    height: 48px;

}
.header__search img{
    width: 17.5px;
    height: 17.5px;
}
.header__search input,input:focus{
    border: 0; 
    width: 1015px;
    outline: none;
    margin-right: 24px;
}

.nav__list{
    display: flex;
    justify-content: center;
    align-items: center;
}
.nav__list li{
    list-style-type: none;
    cursor: pointer;
    margin-right: 20px;
    width: max-content;
}
.nav__list li:hover{
    display:inline-block;
    cursor: pointer;
    color: #73AFF4;
}





</style>

