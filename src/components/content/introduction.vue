<!-- content1  企业介绍---------------------------------------- -->
<template>
    <div class="box">
        <div class="introduction">
            <h2>企业级AI平台解决方案</h2>
            <p>新一代企业级AI平台，携超级智能AI管理助手Cosmic，集感知、思考、行动、智能响应于一体，简化企业管理，提高运营效率，随时在线，随时待命</p>
        <div class="programme">方案详情
            <i class="iconfont icon-jiantoudown"></i>
        </div>
        </div>
        <div class="picture">
            <img src="../../assets/p1.jpg" alt="backgroundImage">
        </div>
    </div>
    
</template>


<script setup>

</script>


<style scoped>
    .box{
        display: flex;
    }
    .introduction{
        margin-top: 50px;
        margin-left: 150px;
    }
    h2{
        font-size: 40px;
    }
    p{
        margin-top: 30px;
        width: 463px;
        margin-bottom: 50px;
    }
    .programme{
        width: 108px;
        /* height: 48px; */
        padding: 10px 10px ;
        background-color: rgb(33, 131, 233);
        color: white;
        text-align: center;
        border-radius: 5px;
    }
    .picture{
        margin-left: 20px;
        /* box-shadow: 50px 30px #ffffff inset; */
        box-shadow: 0 25px 45px rgba(255, 255, 255, 0.1);
        backdrop-filter: blur(4px);
    }
    img{
        width: 800px;
    }
</style>