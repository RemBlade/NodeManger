<template>
    <div>
		<div class="login_main">
            <el-form class="login_form" ref="loginform" :v-model="loginform">
                <h3 class="login_title">云节点管理中心</h3>
                <h3 class="login_title_2">Node Manger System</h3>
                <div class="item_box">
                    <div class="user_name_box">
                        <!-- <span class="user_name_icon_box">
                            <i class="el-icon-user-solid" style="font-size:30px;"></i>
                        </span> -->
                        <el-input prefix-icon="el-icon-user-solid" class="inputDeep" placeholder="请输入用户名" v-model="loginform.username" maxlength="20"></el-input>
                    </div>
                    <div class="password_box">
                        <el-input prefix-icon="el-icon-lock" class="inputDeep" placeholder="请输入密码" v-model="loginform.password" maxlength="20" show-password></el-input>
                    </div>
                    <div class="login_button_box">
                        <el-button class="login_button" @click="login_click">登录</el-button>
                    </div>
                </div>
            </el-form>
        </div>
	
    </div>
</template>

<script>
    export default{
        data() {
            return {
                loginform: {
                    username: "",
                    password: ""
                },

            }
        },
        methods: {
            login_click() {
                console.log(this.loginform.username)
                console.log(this.loginform.password)
            }
        },
    }
</script>

<style scoped>
    .login_main{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        line-height: 1.53846154;
        font-size: 14px;
        font-family: 微软雅黑, Helvetica, Tahoma, Arial, sans-serif;
        color: rgb(0, 0, 0);
        box-sizing: border-box;
        margin-top: -300px;
        margin-left: -200px;
        border-radius: 5px;
        width: 400px;
        position: absolute;
        top: 50%;
        left: 50%;
        background-color: rgba(38,43,54,.9);
        padding: 20px;
        animation-duration: 1s;
        animation-fill-mode: both;
        z-index: 100;
        animation-name: fadeInLeft;
    }   
    .login_form{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        line-height: 1.53846154;
        font-size: 14px;
        font-family: 微软雅黑, Helvetica, Tahoma, Arial, sans-serif;
        color: rgb(0, 0, 0);
        box-sizing: border-box;
        width: 370px;
        margin: 0 auto;
        padding: 20px 30px 13px 23px;
    }
    .login_title{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        box-sizing: border-box;
        font-family: "Helvetica Neue", Helvetica, Tahoma, Arial, 'Microsoft Yahei', 'Hiragino Sans GB', 'WenQuanYi Micro Hei', sans-serif;
        margin-top: 20px;
        margin-bottom: 10px;
        font-size: 26px;
        font-weight: 500;
        padding: 0;
        line-height: 30px;
        text-align: center;
        color: #259dab;
    }
    .login_title_2{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        box-sizing: border-box;
        font-family: "Helvetica Neue", Helvetica, Tahoma, Arial, 'Microsoft Yahei', 'Hiragino Sans GB', 'WenQuanYi Micro Hei', sans-serif;
        margin-top: 10px;
        margin-bottom: 10px;
        font-size: 20px;
        font-weight: 400;
        line-height: 30px;
        text-align: center;
        color: #259dab;
        border-bottom: 1px solid #555;
        padding-bottom: 10px;
    }
    .item_box{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        line-height: 1.53846154;
        font-size: 14px;
        font-family: 微软雅黑, Helvetica, Tahoma, Arial, sans-serif;
        color: rgb(0, 0, 0);
        box-sizing: border-box;
        margin-top: 18px;
    }
    .user_name_box{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        line-height: 1.53846154;
        font-size: 14px;
        font-family: 微软雅黑, Helvetica, Tahoma, Arial, sans-serif;
        color: rgb(0, 0, 0);
        box-sizing: border-box;
        position: relative;
        display: table;
        border-collapse: separate;
        margin-bottom: 15px;
        border-radius: 4px;
        width: 319px;
    }
    .user_name_icon_box{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        font-family: 微软雅黑, Helvetica, Tahoma, Arial, sans-serif;
        border-collapse: separate;
        box-sizing: border-box;
        display: table-cell;
        white-space: nowrap;
        vertical-align: middle;
        padding: 5px 12px;
        font-size: 13px;
        font-weight: normal;
        line-height: 1;
        color: #222;
        text-align: center;
        border-radius: 4px;
        border-top-right-radius: 0;
        border-bottom-right-radius: 0;
        width: 49px;
        border: none;
        background: #fff;
    }
    .user_name_icon{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        border-collapse: separate;
        white-space: nowrap;
        text-align: center;
        box-sizing: border-box;
        display: inline-block;
        font: normal normal normal 14px/1 FontAwesome;
        text-rendering: auto;
        -webkit-font-smoothing: antialiased;
        color: rgba(38,43,54,.9);
        font-size: 24px;
    }
    .inputDeep :deep(.el-input__wrapper) {
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        border-collapse: separate;
        box-sizing: border-box;
        margin: 0;
        font-family: inherit;
        font-size: 13px;
        line-height: 1.53846154;
        vertical-align: middle;
        background-color: #fff;
        transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s, -webkit-box-shadow ease-in-out .15s;
        box-shadow: none;
        border-radius: 0 4px 4px 0;
        position: relative;
        z-index: 2;
        float: left;
        width: 100%;
        margin-bottom: 0;
        display: table-cell;
        border: none;
        border-left: none;
        padding: 10px 20px;
        color: grey;
        height: auto;
        border-top-left-radius: 0;
        border-bottom-left-radius: 0;
    }
    .password_box{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        line-height: 1.53846154;
        font-size: 14px;
        font-family: "微软雅黑",Helvetica,Tahoma,Arial,sans-serif;
        color: #000;
        box-sizing: border-box;
        position: relative;
        display: table;
        border-collapse: separate;
        margin-bottom: 15px;
        border-radius: 4px;
        width: 319px;
    }
    .password_icon_box{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        font-family: "微软雅黑",Helvetica,Tahoma,Arial,sans-serif;
        border-collapse: separate;
        box-sizing: border-box;
        display: table-cell;
        white-space: nowrap;
        vertical-align: middle;
        padding: 5px 12px;
        font-size: 13px;
        font-weight: normal;
        line-height: 1;
        color: #222;
        text-align: center;
        border-radius: 4px;
        border-top-right-radius: 0;
        border-bottom-right-radius: 0;
        width: 43px;
        border: none;
        background: #fff;
    }
    .login_button_box{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        line-height: 1.53846154;
        font-size: 14px;
        font-family: "微软雅黑",Helvetica,Tahoma,Arial,sans-serif;
        color: #000;
        box-sizing: border-box;
        margin: 20px 0 10px;
    }
    .login_button{
        -webkit-text-size-adjust: 100%;
        -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
        box-sizing: border-box;
        margin: 0;
        text-transform: none;
        -webkit-appearance: button;
        font-family: inherit;
        margin-bottom: 0;
        font-weight: normal;
        text-align: center;
        white-space: nowrap;
        vertical-align: middle;
        cursor: pointer;
        user-select: none;
        border-radius: 2px;
        transition: all .4s cubic-bezier(.175, .885, .32, 1);
        color: #fff;
        text-shadow: 0 -1px 0 rgba(0, 0, 0, .2);
        background-color: #08897e;
        padding: 10px 16px;
        font-size: 17px;
        line-height: 1.25;
        display: block;
        width: 100%;
        border: none;
    }

</style>