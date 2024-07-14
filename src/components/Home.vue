<!-- 首页------------------------------------------------- -->
<template>
    <!-- header区域 -->
    <div class="header-top"></div>
    <div class="header">
        <div class="logo">
            <img src="../assets/kingdee2.svg" alt="">
            <img src="../assets/kingdee1.svg" alt="">
            <img src="../assets/kingdee.svg" alt="">
        </div>
        <div class="navigator">
            <Navigator />
        </div>
        <div class="thing">
            <Thing />
        </div>
    </div>

    <!-- content区域 -->
    <div class="content">
        <div class="content1">
            <Introduction />
        </div>
        <div class="content2">
            <More />
        </div>
    </div>
    
</template>

<script setup>
import Navigator from './header/navigator.vue'
import Thing from './header/thing.vue'
import Introduction from './content/introduction.vue';
import More from './content/more.vue';
</script>

<style scoped>
    .header-top{
        height: 27px;
    }
    .header{
        height: 75px;
        display: flex;
    }
    /* logo样式 */
    .logo{
        display: flex;
        width: 154px;
        margin-left: 63px;
    }
    img{
        width: 50px;
    }


    .thing{
        /* width: 400px; */
        flex: 1;
        margin-left: 170px;
    }
</style>
