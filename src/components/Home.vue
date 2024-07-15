<!-- 首页--------------------------------------------------------- -->
<template>
    <div class="content_warp">
        <div class="content">
            <div class="header_nav">
                <div class="header_top">

                </div>
                <div class="header_content">
                    <!-- 语言选择、登录、注册  -->
                    <div class="header_phone">
                        <div class="header_language_left">
                            <div @mouseleave="mouseLeaveRegion">
                                <img src="../assets/earth.svg" alt="language_logo" @mouseenter="mouseOverRegion" >
                                <div class="region"  :class=" showRegion ? 'region_hover' : '' "  >
                                    <a href="#">简体中文</a>
                                    <a href="#">繁体中文</a>
                                    <a href="#">English</a>
                                </div>
                            </div>
                        </div>
                        <div class="header_loginAndregister_right">
                            <a href="#" class="header_login_right">
                                登录
                            </a>
                            |
                            <a href="#" class="header_register_right">
                                注册
                            </a>                      
                        </div>
                    </div>
                    <!-- 金蝶logo -->
                    <div class="header_logo">
                        <img src="../assets/logohei.gif" alt="">
                    </div>
                    <!-- 导航栏 -->
                    <div class="header_navigator">
                        <ul class="nav_list">
                            <li 
                                class="nav_item" 
                                v-for="(item,index) of navigator_table_data" 
                                :key="index"
                                @mouseover="hoverNav(index)" >
                                <a href="item.href">{{ item.name }}</a>
                                <div class="line"></div>
                                <div 
                                    class="nav_sec"
                                    v-show="navShowIndex === index ">
                                    <!-- {{ item2.name }} -->
                                    <ul class="nav_sec_left">
                                        <li 
                                            v-for="item2 of item.navigator_table_data2" 
                                            :key="item2.id">
                                            {{ item2.name }}
                                        </li>
                                        <a href="#">查看所有产品 > </a>
                                        <p>销售热线： 4008-830-830</p>
                                    </ul>
                                    <ul class="nav_sec_right">
                                        <li
                                            v-for="item3 of item.navigator_table_data3"
                                            :key="item3.id">
                                            {{ item3.name }}
                                        </li>
                                    </ul>
                                </div>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<script setup>
import { ref } from 'vue'
import '../style.css'
   
    // 语言选择、登录、注册  
    const showRegion = ref(false);
    const mouseOverRegion = () => {
        showRegion.value = true;
    };
    const mouseLeaveRegion = () => {
        showRegion.value = false;
        console.log("🚀 ~ mouseLeaveRegion ~ mouseLeaveRegion:", mouseLeaveRegion);
    };

    // 导航栏
    const navigator_table_data = [
        {
            id:'1',
            name:'产品',
            navigator_table_data2:[
                {
                    id:'1-1',
                    name:'业务领域'
                },
                {
                    id:'1-2',
                    name:'企业级AI平台',
                    detail:[
                        {
                            id:'1-2-1',
                            name:'开发服务云',
                            description:'低代码平台,高敏捷,动态领域模型'
                        },
                        {
                            id:'1-2-2',
                            name:'流程服务云',
                            description:'灵活、高效、可靠的流程全生命周期管理'
                        },
                        {
                            id:'1-2-3',
                            name:'集成服务云',
                            description:'低代码开发平台和配置平台,可视化配置'
                        },
                        {
                            id:'1-2-4',
                            name:'数据服务云',
                            description:'数据分析和数据探索平台纵'
                        },
                        {
                            id:'1-2-5',
                            name:'区块链服务云',
                            description:'低代码模式的“一站式”企业级区块链服务'
                        },
                        {
                            id:'1-2-6',
                            name:'AI服务云',
                            description:'实现各场景智能化应用打造企业级AI服务'
                        },
                        {
                            id:'1-2-7',
                            name:'RPA服务云',
                            description:'安全、可靠、稳定的虚拟数字员工生产力'
                        },
                        {
                            id:'1-2-8',
                            name:'数据中台',
                            description:'原始数据转为数据资产，构建数据服务'
                        },
                        {
                            id:'1-2-9',
                            name:'国际化',
                            description:'支持本地化合规，提升海外用户体验'
                        },
                        {
                            id:'1-2-10',
                            name:'云基础平台',
                            description:'提供开发、运维一体化管理平台'
                        }      
                    ]
                },
                {
                    id:'1-3',
                    name:'大型企业',
                    detail:[
                        {
                            id:'1-3-1',
                            name:'人力云',
                            description:'激活人人，共建组织韧性'
                        },
                        {
                            id:'1-3-2',
                            name:'财务云',
                            description:'重构数字战斗力，助力大企业财务转型'
                        },
                        {
                            id:'1-3-3',
                            name:'税务云',
                            description:'“业财税票资档”一体化数字化税控体系'
                        },
                        {
                            id:'1-3-4',
                            name:'供应链云',
                            description:'共生商业、智能运营、共享中台'
                        },
                        {
                            id:'1-3-5',
                            name:'制造云',
                            description:'精益制造 智能互联 生态协同 数字运营'
                        },
                        {
                            id:'1-3-6',
                            name:'营销云',
                            description:'全域营销+数智化协同管理方案'
                        },
                        {
                            id:'1-3-7',
                            name:'采购云',
                            description:'降低采购业务成本，增强供应韧性'
                        },
                        {
                            id:'1-3-8',
                            name:'协同云 ',
                            description:'业务协同一体化，提升企业运转效率'
                        },
                        {
                            id:'1-3-9',
                            name:'发票云',
                            description:'发票管理及协同服务、影像及电子会计档案管理'
                        }   
                    ]
                },
                {
                    id:'1-4',
                    name:'高成长型企业',
                    detail:[
                        {
                            id:'1-1-1',
                            name:'财务云',
                            description:'财务和业务高效协同，支撑业务敏捷创新'
                        },
                        {
                            id:'1-1-2',
                            name:'税务云',
                            description:'“业财税票资档”一体化智慧税务管理'
                        },
                        {
                            id:'1-1-3',
                            name:'人力云',
                            description:'基于全球领先实践打造的人力资源管理平台'
                        },
                        {
                            id:'1-1-4',
                            name:'制造云',
                            description:'纵向集成、端到端集成、横向集成'
                        },
                        {
                            id:'1-1-5',
                            name:'供应链云',
                            description:'实现供应链可视化管理'
                        },
                        {
                            id:'1-1-6',
                            name:'星域工业互联网',
                            description:'入选国家级“双跨”平台'
                        },
                        {
                            id:'1-1-7',
                            name:'全渠道云',
                            description:'覆盖电商、零售、渠道、分销全业务场景'
                        },
                        {
                            id:'1-1-8',
                            name:'协同办公云 ',
                            description:'协同门户、协同审批、智能签到、知识中心等'
                        },
                        {
                            id:'1-1-9',
                            name:'发票云',
                            description:'发票管理及协同服务、影像及电子会计档案管理'
                        }   
                    ]
                },
                {
                    id:'1-5',
                    name:'小微型企业',
                    detail:[
                        {
                            id:'1-1-1',
                            name:'财务云',
                            description:'财务和业务高效协同，支撑业务敏捷创新'
                        },
                        {
                            id:'1-1-2',
                            name:'税务云',
                            description:'“业财税票资档”一体化智慧税务管理'
                        },
                        {
                            id:'1-1-3',
                            name:'人力云',
                            description:'基于全球领先实践打造的人力资源管理平台'
                        },
                        {
                            id:'1-1-4',
                            name:'制造云',
                            description:'纵向集成、端到端集成、横向集成'
                        },
                        {
                            id:'1-1-5',
                            name:'供应链云',
                            description:'实现供应链可视化管理'
                        },
                        {
                            id:'1-1-6',
                            name:'星域工业互联网',
                            description:'入选国家级“双跨”平台'
                        },
                        {
                            id:'1-1-7',
                            name:'全渠道云',
                            description:'覆盖电商、零售、渠道、分销全业务场景'
                        },
                        {
                            id:'1-1-8',
                            name:'协同办公云 ',
                            description:'协同门户、协同审批、智能签到、知识中心等'
                        },
                        {
                            id:'1-1-9',
                            name:'发票云',
                            description:'发票管理及协同服务、影像及电子会计档案管理'
                        }   
                    ]
                },             
            ],
            navigator_table_data3:[
                        {
                            id:'1-1-1',
                            name:'财务云',
                            description:'财务和业务高效协同，支撑业务敏捷创新'
                        },
                        {
                            id:'1-1-2',
                            name:'税务云',
                            description:'“业财税票资档”一体化智慧税务管理'
                        },
                        {
                            id:'1-1-3',
                            name:'人力云',
                            description:'基于全球领先实践打造的人力资源管理平台'
                        },
                        {
                            id:'1-1-4',
                            name:'制造云',
                            description:'纵向集成、端到端集成、横向集成'
                        },
                        {
                            id:'1-1-5',
                            name:'供应链云',
                            description:'实现供应链可视化管理'
                        },
                        {
                            id:'1-1-6',
                            name:'星域工业互联网',
                            description:'入选国家级“双跨”平台'
                        },
                        {
                            id:'1-1-7',
                            name:'全渠道云',
                            description:'覆盖电商、零售、渠道、分销全业务场景'
                        },
                        {
                            id:'1-1-8',
                            name:'协同办公云 ',
                            description:'协同门户、协同审批、智能签到、知识中心等'
                        },
                        {
                            id:'1-1-9',
                            name:'发票云',
                            description:'发票管理及协同服务、影像及电子会计档案管理'
                        }   
                    ]
        },
        {
            id:'2',
            name:'行业解决方案'
        },
        {
            id:'3',
            name:'标杆案例'
        },
        {
            id:'4',
            name:'服务支持'
        },
        {
            id:'5',
            name:'应用市场'
        },
        {
            id:'6',
            name:'生态伙伴与开发者'
        },
        {
            id:'7',
            name:'关于金蝶'
        },
    ];
    
    let navShowIndex = 0;
    const hoverNav = (index) => {
        navShowIndex = index;
        console.log(navShowIndex);
    }


</script>


<style lang="scss" scoped>
    .content_warp, body{
        width: 100%;
        min-height: 100vh;
        background-color: antiquewhite;
        .content{
            width: 1080px;
            min-width: 800px;
            margin: 0 auto;
            min-height: 100vh;
            
        }

        @media screen and (min-width: 600px){
            .content{
                width: 600px;
            }
        }
        @media screen and (min-width: 1000px){
            .content{
                width: 1100px;
            }
        }
        @media screen and (min-width: 1280px){
            .content{
                width: 1360px;
            }
        }
        @media screen and (min-width: 2200px){
            .content{
                width: 2000px;
            }
        }

        a {
            text-decoration: none; /* 去除默认的下划线 */
            outline: none;	/* 去除旧版浏览器的点击后的外虚线框 */
            color: rgb(87, 93, 108);	/* 去除默认的颜色和点击后变化的颜色 */ 
        }

    }
    

    .header_top{
        height: 27px;
        background-color: white;
    }
    .header_content{
        position: relative;
        .header_phone{
            position: absolute;
            background-color: white;
            display: inline-block;
            width: 146px;
            right: 0px;
            .header_language_left{
                display: inline-block;
                margin-left: -2px;
                img{
                    width: 26px;
                    height: 26px;
                }
                .region{
                    position: absolute;
                    background-color: rgb(255, 255, 255);
                    width: 96px;
                    height: 0px;
                    right: 78px;
                    top: 28px;
                    color: rgb(87, 93, 108);
                    font-family: PingFangM, Arial, sans-serif;
                    font-size: 14px;
                    box-shadow: rgba(0, 0, 0, 0.2) 0px 10px 15px 0px;
                    transition: all 0.5s ease-out;
                    overflow: hidden;
                    a{
                        display: block;
                        padding-top: 13px;
                        padding-bottom: 13px;
                        text-align: center;
                    }
                    :nth-child(1){
                        margin-top: 9px;
                    }
                }
                .region_hover{
                    height: 150px;
                }
                a:hover{
                    color: white;
                    background-color: rgb(33, 131, 233);
                }
            }
            .header_loginAndregister_right{
                display: inline-block;
                top: -8px;
                right: -23px;
                position: relative;
                font-size: 14px;
                color: rgb(87, 93, 108);
                
                .header_login_right{
                    display: inline-block;
                }
                .header_register_right{
                    display: inline-block;
                }
            }
        }

        .header_logo{
            position: absolute;
            left: 30px;
            img{
                width: 182px;
            }
        }

        .header_navigator{
            position: absolute;
            top: 28px;
            left: 204px;
            width: 100%;
            .nav_list{
                display: inline-block;
                .nav_item{
                    display: inline-block;
                    position: relative;
                    a{
                        color: rgb(37, 43, 58);
                        padding: 10px;
                        font-size: 14px;
                    }
                    .line{
                        position: absolute;
                        top: 47px;
                        width: 0;
                        left: 50%;
                        height: 2px;
                        background-color: rgb(33, 131, 233);
                        transition: all 0.2s ease-in-out;
                    }
                    .nav_sec{
                        position: absolute;
                        height: 480px;
                        width: 267px;
                        left: -153px;
                        top: 49px;
                        background-color: rgb(246, 247, 251);
                        border-top: 1px solid lightgray;
                        font-family: PingFangM, Arial, sans-serif;
                        color: rgb(37, 43, 58);
                        .nav_sec_left{
                            position: absolute;
                            display: inline-block;
                            width: 100%;
                            li{
                                padding: 21px 40px 21px 39px;
                                font-size: 18px;       
                            }
                            li:hover{
                                color: rgb(4, 103, 207);
                                background-color: white;
                            }
                            a{
                                display: inline-block;
                                font-size: 14px; 
                                margin-top: 69px;
                                margin-left: 29px;
                                color: black;
                            }
                            a:hover{
                                color: rgb(4, 103, 207);
                            }
                            p{
                                display: inline-block;
                                font-size: 12px;
                                margin-left: 39px;
                            }
                        }
                        .nav_sec_right{
                            position: absolute;
                            display: inline-block;
                            width: 348%;
                            background-color:aqua;
                            border-top: 1px solid lightgray;
                            top: -1px;
                            height: 480px;
                            left: 267px;
                            li{
                                padding: 10px;
                                font-size: 18px; 
                                display: inline-block;      
                            }
                        }
                    }
                }
                .nav_item:hover .line{
                    width: 100%;
                    left: 0;
                }
            }
        }
    }
   
    
</style>








