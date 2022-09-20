<template>
    <div id="index-page">
        <el-container>
            <el-aside class="aside">
                <el-menu>
                    <el-menu-item index="1-1" class="menu_top">Node Manger </el-menu-item>
                    <el-menu-item index="1-2" class="menu_item">
                        <i class="el-icon-s-platform"></i>
                        节点概况
                    </el-menu-item>
                    <el-menu-item index="1-3" class="menu_item">
                        <i class="el-icon-s-grid"></i>
                        节点详情
                    </el-menu-item>
                </el-menu>
                    
            </el-aside>
            <el-container>
                <el-header class="header">
                    <div class="icon">
                        <i class="el-icon-s-custom"></i>
                    </div>
                </el-header>
            </el-container>
        </el-container>
    </div>
</template>

<script>
    export default {
        components: {
            
        },
        data() {
            return {
            }
        }
    }
</script>

<style scoped>
    .icon{
        position: absolute;top:50%;
        left:99%;
        transform:translate(-50%,-50%);
    }
    .header{
        background: #323232;
        text-align: right;
        margin-right: 5px;
        color:#F09B22;
        font-size: 20px;
        position:relative;
    }
    /* .header{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0,0,0,0);
        font-size: 14px;
        line-height: 1.42857143;
        color: #333;
        font-family: 'Open Sans', sans-serif;
        box-sizing: border-box;
        display: block;
        min-height: 50px;
        position: fixed;
        width: 100%;
        z-index: 300;
        box-shadow: 0 3px 3px rgba(0, 0, 0, 0.05);
        margin: 0px;
        background: #323232;
        border: 0px solid black;
        border-radius: 0px;
    } */
    .menu_top{
        font-family: 'Open Sans', sans-serif;
        color: white;
        width: 300px;
        text-align: left;
        height: 60px;
        font-size: 24px;
        font-weight: 700;
        /* line-height: 30px; */
        background: #F09B22;
        margin: 0 auto;
    }
    .menu_item{
        font-size: 14px;
        font-family: 'Open Sans', sans-serif;
        list-style: none;
        box-sizing: border-box;
        text-decoration: none;
        background-color: #1B1B1B !important;
        color: #F09B22 !important;
        position: relative;
        display: block;
        background: transparent;
    }
    .aside{
        height: 100vh;
        background: #323232;
    }
</style>
