<!-- 导航栏------------------------------------------------- -->
<template>
    <!-- 导航栏 -->
    <!-- <el-menu mode="horizontal" :ellipsis="false">
        <el-sub-menu index="1">
            <template #title>产品</template>
            <el-sub-menu index="1-1">
                <template #title>业务领域</template>
                <h2>业务领域</h2>
                <el-menu-item index="2-1">财务云</el-menu-item>
                <el-menu-item index="2-2">税务云</el-menu-item>
                <el-menu-item index="2-3">人力云</el-menu-item>
                <el-menu-item index="2-4">制造云</el-menu-item>
                <el-menu-item index="2-5">供应链云</el-menu-item>
                <el-menu-item index="2-6">星域工业互联网</el-menu-item>
                <el-menu-item index="2-7">全渠道云</el-menu-item>
                <el-menu-item index="2-8">协同办公云</el-menu-item>
                <el-menu-item index="2-9">发票云</el-menu-item>
            </el-sub-menu>
            <el-sub-menu index="1-2">
                <template #title>企业级AI平台</template>
                <h2>金蝶云·苍穹 企业级AI平台 ></h2>
                <el-menu-item index="2-1">开发服务云</el-menu-item>
                <el-menu-item index="2-2">流程服务云</el-menu-item>
                <el-menu-item index="2-3">集成服务云</el-menu-item>
                <el-menu-item index="2-4">数据服务云</el-menu-item>
                <el-menu-item index="2-5">区块链服务云</el-menu-item>
                <el-menu-item index="2-6">AI服务云</el-menu-item>
                <el-menu-item index="2-7">RPA服务云</el-menu-item>
                <el-menu-item index="2-8">数据中台</el-menu-item>
                <el-menu-item index="2-9">国际化</el-menu-item>
                <el-menu-item index="2-10">云基础平台</el-menu-item>
            </el-sub-menu>
            <el-sub-menu index="1-3">
                <template #title>大型企业</template>
                <h2>金蝶云·星瀚 大型企业SaaS管理云 ></h2>
                <el-menu-item index="2-1">人力云</el-menu-item>
                <el-menu-item index="2-2">财务云</el-menu-item>
                <el-menu-item index="2-3">税务云</el-menu-item>
                <el-menu-item index="2-4">供应链云</el-menu-item>
                <el-menu-item index="2-5">制造云</el-menu-item>
                <el-menu-item index="2-6">营销云</el-menu-item>
                <el-menu-item index="2-7">采购云</el-menu-item>
                <el-menu-item index="2-8">协同云</el-menu-item>
                <h2>金蝶EAS Cloud 集团企业数字化解决方案 ></h2>
                <el-menu-item index="2-9">s-HR Cloud</el-menu-item>
                <el-menu-item index="2-10">财务共享</el-menu-item>
                <el-menu-item index="2-11">司库管理</el-menu-item>
                <el-menu-item index="2-12">税务管理</el-menu-item>
                <el-menu-item index="2-13">采购管理</el-menu-item>
                <el-menu-item index="2-14">全面预算</el-menu-item>
                <el-menu-item index="2-15">销售管理</el-menu-item>
            </el-sub-menu>
            <el-sub-menu index="1-4">
                <template #title>高成长型企业</template>
                <h2>金蝶云·星空旗舰版 新一代高成长型企业SaaS管理云 ></h2>
                <el-menu-item index="2-1">财务云</el-menu-item>
                <el-menu-item index="2-2">税务云</el-menu-item>
                <el-menu-item index="2-3">员工服务云</el-menu-item>
                <el-menu-item index="2-4">全渠道云</el-menu-item>
                <el-menu-item index="2-5">采购云</el-menu-item>
                <el-menu-item index="2-6">供应链云</el-menu-item>
                <el-menu-item index="2-7">PLM云</el-menu-item>
                <el-menu-item index="2-8">制造云</el-menu-item>
                <el-menu-item index="2-9">项目云</el-menu-item>
                <el-menu-item index="2-10">数据智能云</el-menu-item>
                <h2>金蝶云·星空 高成长型企业SaaS管理云 ></h2>
                <el-menu-item index="2-11">财务云</el-menu-item>
                <el-menu-item index="2-12">供应链云</el-menu-item>
                <el-menu-item index="2-13">全渠道云</el-menu-item>
                <el-menu-item index="2-14">制造云</el-menu-item>
                <el-menu-item index="2-15">PLM云</el-menu-item>
                <el-menu-item index="2-16">餐饮云</el-menu-item>
                <el-menu-item index="2-17">数据服务云</el-menu-item>
            </el-sub-menu>
            <el-sub-menu index="1-5">
                <template #title>小微型企业</template>
                <h2>金蝶云·星辰 小型企业SaaS管理云 ></h2>
                <el-menu-item index="2-1">进销存</el-menu-item>
                <el-menu-item index="2-2">财税管理</el-menu-item>
                <el-menu-item index="2-3">费用报销</el-menu-item>
                <el-menu-item index="2-4">零售管理</el-menu-item>
                <el-menu-item index="2-5">生产管理</el-menu-item>
                <el-menu-item index="2-6">电商云</el-menu-item>
                <el-menu-item index="2-7">订货商城</el-menu-item>
                <h2>金蝶精斗云 微型企业SaaS管理云 ></h2>
                <el-menu-item index="2-8">云会计</el-menu-item>
                <el-menu-item index="2-9">云进销存</el-menu-item>
                <el-menu-item index="2-10">云报销</el-menu-item>
                <h2>金蝶KIS云 小微企业管理上云解决方案 ></h2>
            </el-sub-menu>
        </el-sub-menu>

        <el-sub-menu index="2">
            <template #title>行业解决方案</template>
            <el-sub-menu index="2-1">
                <template #title>热点方案</template>
                <el-menu-item index="2-1">企业级AI平台解决方案</el-menu-item>
                <el-menu-item index="2-2">企业出海数字化方案</el-menu-item>
                <el-menu-item index="2-3">央国企数字化解决方案</el-menu-item>
                <el-menu-item index="2-4">专精特新企业数字化方案</el-menu-item>
                <el-menu-item index="2-5">数字化转型方法论</el-menu-item>
                <el-menu-item index="2-6">小微企业业财税一体化方案</el-menu-item>
                <el-menu-item index="2-7">EBC下一代ERP</el-menu-item>
                <el-menu-item index="2-8">企业IPO解决方案</el-menu-item>
            </el-sub-menu>
            <el-sub-menu index="2-2">
                <template #title>行业方案</template>
                <el-menu-item index="2-1">开发服务云</el-menu-item>
                <el-menu-item index="2-2">流程服务云</el-menu-item>
                <el-menu-item index="2-3">集成服务云</el-menu-item>
                <el-menu-item index="2-4">数据服务云</el-menu-item>
                <el-menu-item index="2-5">区块链服务云</el-menu-item>
                <el-menu-item index="2-6">AI服务云</el-menu-item>
                <el-menu-item index="2-7">RPA服务云</el-menu-item>
                <el-menu-item index="2-8">数据中台</el-menu-item>
                <el-menu-item index="2-9">国际化</el-menu-item>
                <el-menu-item index="2-10">云基础平台</el-menu-item>
            </el-sub-menu>
        </el-sub-menu>
        <el-menu-item index="3">标杆案例</el-menu-item>
        <el-sub-menu index="4">
            <template #title>服务支持</template>
            <el-table :data="serviceSupportTableData" class="serviceSupportTable" style="width: 600px;--el-table-border-color: none; ">
                <el-table-column prop="about" label="关于客户成功"/>
                <el-table-column prop="service" label="客户成功服务"/>
                <el-table-column prop="eac" label="赋能与认证"/>
                <el-table-column prop="notice" label="公告"/>
            </el-table>
        </el-sub-menu>
        <el-menu-item index="5">应用市场</el-menu-item>
        <el-sub-menu index="6">
            <template #title>生态伙伴与开发者</template>
            <el-table :data="partnerTableData" class="partnerTable" style="width: 600px;--el-table-border-color: none; ">
                <el-table-column prop="tobe" label="成为合作伙伴"/>
                <el-table-column prop="search" label="查询合作伙伴"/>
                <el-table-column prop="develop" label="开发者"/>
                <el-table-column prop="tae" label="技术与赋能"/>
            </el-table>
        </el-sub-menu>
        <el-sub-menu index="7">
            <template #title>关于金蝶</template>
            <el-table :data="aboutTableData1" class="aboutTable1" style="width: 750px;--el-table-border-color: none; ">
                <el-table-column prop="about" label="了解金蝶"/>
                <el-table-column prop="news" label="新闻与活动"/>
                <el-table-column prop="manage" label="中国管理模式"/>
                <el-table-column prop="meeting" label="创见者大会"/>
            </el-table>
            <el-table :data="aboutTableData2" class="aboutTable2" style="width: 750px;--el-table-border-color: none; ">
                <el-table-column prop="esg" label="ESG"/>
                <el-table-column prop="investor" label="投资者关系"/>
                <el-table-column prop="recruit" label="金蝶招聘"/>
                <el-table-column prop="contact" label="联系我们"/>
            </el-table>
        </el-sub-menu>

    </el-menu> -->

    <div class="menu">
        <div class="menuNavigator">
            <div v-for="item of navigatorTable" :key="item.id" class="title">
                {{ item.name }}
                <div class="list">
                    <div v-for="list of item.navigatorListTable" :key="list.id" class="listInformation">
                        {{ list.name }}
                        <div class="content">
                            <p v-for="sub of list.navigatorSubTable" :key="sub.id">{{ sub.name }}</p>
                            <div class="contentInformation">
                                <img src="#" alt="">
                                <div href="#" v-for="content of list.navigatorContentTable" :key="content.id" class="contentList">{{ content.name }}</div>
                                <p></p>
                            </div>
                        </div>
                    </div>    
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { get } from 'vant/lib/utils';
import { ref,reactive } from 'vue';

    // const serviceSupportTableData = [
    //     { about:'客户成功体系' , service:'服务产品与方案', eac:'金蝶认证', notice:'服务公告' },
    //     { about:'' , service:'我的服务', eac:'数字化人才赋能', notice:'产品生命周期' },
    //     { about:'' , service:'金蝶云社区', eac:'数字化转型工作坊', notice:'安全通告' }
    // ];
    // const partnerTableData = [
    //     { tobe:'金蝶伙伴体系' , search:'伙伴资质查询', develop:'开发文档', tae:'伙伴生态圈' },
    //     { tobe:'营销服务伙伴' , search:'', develop:'工具与赋能', tae:'' },
    //     { tobe:'专业服务伙伴' , search:'', develop:'在线课程', tae:'' },
    //     { tobe:'独立软件开发' , search:'', develop:'开发者社区', tae:'' },
    //     { tobe:'技术平台伙伴' , search:'', develop:'开发者大赛', tae:'' },
    //     { tobe:'院线联盟' , search:'', develop:'', tae:'' }
    // ];
    // const aboutTableData1 = [
    //     { about:'集团介绍' , news:'新闻动态', manage:'中国管理模式杰出奖', meeting:'关于创见者' },
    //     { about:'懂事及管理层' , news:'市场活动', manage:'十三届中国管理全球论坛', meeting:'2023全球创见者大会' },
    //     { about:'发展历程' , news:'媒体报告', manage:'十二届中国管理全球论坛', meeting:'2022全球创见者大会' },
    //     { about:'公司荣誉' , news:'社交媒体', manage:'十一届中国管理全球论坛', meeting:'2021全球创见者大会' },
    //     { about:'社会责任' , news:'', manage:'十届中国管理全球论坛', meeting:'' },
    //     { about:'信任中心' , news:'', manage:'', meeting:'' }
    // ];
    // const aboutTableData2 = [
    //     { esg:'ESG报告' , investor:'投资者关系主页', recruit:'校园招聘', contact:'总部及分支结构' },
    //     { esg:'' , investor:'公告与通函', recruit:'社会招聘', contact:'购买与咨询' },
    //     { esg:'' , investor:'财务报告', recruit:'成长与发展', contact:'' },
    //     { esg:'' , investor:'股票信息', recruit:'生活在金蝶', contact:'' }
    // ];

    const navigatorTable = [
        { 
            id:'1',
            name:'产品',
            navigatorListTable:[
                { 
                    id:'1-1',
                    name:'业务领域',
                    navigatorSubTable:[
                        {
                            id:'1-1-1-1',
                            name:'业务领域',
                        }
                    ],
                    navigatorContentTable:[
                        { id:'1-1-1',name:'财务云' },
                        { id:'1-1-2',name:'税务云' },
                        { id:'1-1-3',name:'人力云' },
                        { id:'1-1-4',name:'制造云' },
                        { id:'1-1-5',name:'供应链云' },
                        { id:'1-1-6',name:'星域工业互联网' },
                        { id:'1-1-7',name:'全渠道云' },
                        { id:'1-1-8',name:'协同办公云' },
                        { id:'1-1-9',name:'发票云' }
                    ]
                },
                { id:'1-2',name:'企业级AI平台' },
                { id:'1-3',name:'大型企业' },
                { id:'1-4',name:'高成长型企业' },
                { id:'1-5',name:'小微型企业' },
                { id:'1-6',name:'查看所有产品' },
                { id:'1-7',name:'销售热线： 4008-830-830' },
            ]
        },
        { id:'2',name:'行业解决方案' },
        { id:'3',name:'标杆案例' },
        { id:'4',name:'服务支持' },
        { id:'5',name:'应用市场' },
        { id:'6',name:'生态伙伴与开发者' },
        { id:'7',name:'关于金蝶' }
    ]
  
    
 
</script>

<style scoped>
    .menu{
        width: 100%;
        margin-top: 18px;
        margin-left: 29px;
    }
    .title{
        display: inline;
        white-space: nowrap;
        font-size: 14px;
        padding: 8px;
        padding-bottom: 25px;
        color: rgb(37, 43, 58);
        /* background-color: aqua; */
    }
    .title:hover{
        border-bottom: 2px solid rgb(0, 104, 221);
    }
    .list{
        width: 275px;
        height: 480px;
        position: absolute;
        top: 102px;
        left: 92px;
        border-top: 1px solid transparent;
        /* box-shadow: rgba(180, 180, 180, 0.158) -3px 12px 15px 0px; */
        /* background-color: rgb(255, 255, 255); */
        display: none;
    }
    .title:hover .list{
        display: block;
    }
    .title:hover .list,.title:hover .content{
        border-top: 1px solid lightgray;
    }
    /* .list :not(.listInformation){
        background-color: inherit;
    } */
    .listInformation{
        cursor: pointer;
        background-color: rgb(245, 247, 250);
        font-size: 18px;
        font-family: PingFangM, Arial, sans-serif;
        text-align: left;
        line-height: 27px;
        padding: 18px 10px 14px 35px;
        color: rgb(37, 43, 58);
    }
    .listInformation:hover{
        color: rgb(0, 104, 221);
        background-color: white;
    }
    /* .list :nth-child(1) + :not(.content){
        background-color: antiquewhite;
    } */
    /* .list :nth-child(1) + :not(.content) + :hover{
        background-color: antiquewhite;
    } */
    .list :nth-child(6){
        padding-top: 79px; 
        padding-bottom: 0px;
        font-size: 14px;
        background-color: rgb(255, 255, 255);
        color: rgb(37, 43, 58);
    } 
    .list :nth-child(7){
        font-size: 12px;
        padding-top: 6px;
        padding-bottom: 46px;
        background-color: rgb(255, 255, 255);
        color: rgb(37, 43, 58);
    } 
    .content{
        width: 918px;
        height: 481px;
        position: absolute;
        /* background-color: rgba(255, 255, 255, 0.088); */
        border-top: 1px solid transparent;
        left: 275px;
        top: -1px;
        z-index:1;
        /* box-shadow: rgba(180, 180, 180, 0.158) 3px 12px 15px 0px; */
        
    }
    /* .content :not(p){
        background-color: inherit;
    } */
    .contentInformation{
        display: flex;
        z-index: 999 !important;
    }
    .contentInformation :nth-child(6){
        font-size: 16px;
        font-family: PingFangM, Arial, sans-serif;
        text-align: left;
        line-height: 27px;
        padding: 10px;
        color: rgb(37, 43, 58);
    }
    .contentInformation :nth-child(7){
        font-size: 16px;
        font-family: PingFangM, Arial, sans-serif;
        text-align: left;
        line-height: 27px;
        padding: 10px;
        color: rgb(37, 43, 58);
    }
    .content p{
        z-index: 999 !important;
        padding-left: 24px;
        padding-top: 6px;
    }
    .contentList{
        padding: 10px;
        font-size: 16px;
        flex-wrap: wrap;
    }

</style>