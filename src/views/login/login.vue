<template>
 <div class="container">
     <van-nav-bar title="登录"/>
     <van-cell-group>
    <van-field
        v-model="username"
        required
        clearable
        label="手机号"
        left-icon="phone-circle-o"

        placeholder="请输入手机号"
    />

    <van-field
        v-model="password"
        type="password"
        label="验证码"
        placeholder="请输入验证码"
        left-icon="comment-circle-o"
        required
    >
        <van-button class="btn" slot="button" size="small" type="primary">发送验证码</van-button>
    </van-field>
    </van-cell-group>
    <div style="padding:20px">
         <van-button type="info" style="width:100%;border-radius:10px">登录</van-button>
    </div>
 </div>
</template>

<script>
export default {

}
</script>

<style copend lang="less">
    .container{
        position:absolute;
        width: 100%;
        height: 100%;
        top:0;
        left:0;
        background-color: #eee;
        .btn {
            background: #777777;
            border-radius:15px;
        }
        .van-cell:not(:last-child)::after{
            background: #666;
            right: 16px;
        }
    }
</style>
