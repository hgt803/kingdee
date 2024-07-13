<!-- header右侧组件------------------------------------------------------------ -->
<template>
    <!-- 登录和注册------------------------------------------------- -->
    <div class="loginAndregister">
        <img src="../../assets/earth.svg" alt="">
        <div class="larText">
            登录 | 注册
        </div>
    </div>
    <!-- 联系电话，申请体验，搜索框------------------------------------------------- -->
    <div class="things">
        <div class="phone">
            <img src="../../assets/phone.svg" alt="">
            <p>4008-830-830</p>
        </div>
        <div class="applyButton">
            <button type="submit">申请体验</button>
        </div>
        <div class="search">
            <img src="../../assets/magnifier.svg" alt="">
        </div>
    </div>
    
</template>

<script setup>
import { ref } from 'vue';

    
</script>

<style scoped>
    /* 登录和注册样式 */
    .loginAndregister{
        width: 150px;
        margin-top: -15px;
        margin-left: 243px;
        display: flex;
    }
    .loginAndregister img{
        width: 24px;
    }
    .larText{
        margin-left: 24px;
        font-size: 14px;
        color: rgb(87, 93, 108);
    }

    /* 联系方式、申请体验、搜索框样式 */
    .things{
        display: flex;
        margin-left: 55px;
    }
    .things div{
        justify-content: center;
        align-items: center;
    }
    .phone{
        display: flex;
        margin-top: 5px;
    }
    .phone img{
        margin-right: 4px;
        width: 25px;
        transform: rotate(0.98turn);
    }
    .phone p{
        font-size: 14px;
        color: rgb(87, 93, 108);
    }
    .applyButton{
        margin-top: 10px;
        margin-left: 25px;
    }
    .applyButton button{
        width: 98px;
        height: 38px;
        background-color: white;
        border: 1px lightgray solid;
        border-radius: 5px;
        font-size: 14px;
        color: rgb(0, 104, 221);
    }
    .applyButton button:hover{
        background-color: rgb(0, 104, 221);
        color: white;
    }
    .search{
        margin-top: 15px;
        margin-left: 30px;
    }
    .search img{
        width: 25px;
    }
    
</style>

