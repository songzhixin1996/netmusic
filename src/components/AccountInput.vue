<template>
    <div class="my-input">
        <div class="account">
            <span>icon/+86</span>
            <input type="tel" maxlength="11" placeholder="请输入手机号" v-model="account">
        </div>
        <div class="password">
            <span>icon</span>
            <input type="password" maxlength="40" placeholder="请输入密码" v-model="password">
            <router-link to="forgetPassword">忘记密码?</router-link>
        </div>
    </div>
</template>
<script>
export default {
    props: ['account', 'password']
};
</script>


<style lang="scss" scoped>
.my-input input {
    border: none;
    outline: none;
    padding-left: 3%;
}
.account,
.password {
    padding-bottom: 1%;
    border-bottom: 1px solid gray;
    margin: 10% 5%;
    a {
        float: right;
        color: rgb(53, 91, 173);
        text-decoration: none;
        padding-right: 2%;
    }
}
</style>
