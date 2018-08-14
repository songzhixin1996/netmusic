<template>
    <div class="login">
        <div class="logo">
            <img src="../assets/logo.jpg">
        </div>
        <div class="select">
            <div>
                <router-link to="phonelogin">手机号登录</router-link>
            </div>
            <div>
                <router-link to="regist">注册</router-link>
            </div>
            <div>
                <router-link to="asd">
                    <span>游客试用</span>
                </router-link>
            </div>
        </div>
        <div class="other">
            <div>其他登录方式</div>
            <div class="other-list">
                <div class="other-item"><img src="../assets/logo.jpg"><br/>wb</div>
                <div class="other-item"><img src="../assets/logo.jpg"><br/>qq</div>
                <div class="other-item"><img src="../assets/logo.jpg"><br/>wb</div>
                <div class="other-item"><img src="../assets/logo.jpg"><br/>wy</div>
            </div>
        </div>
    </div>

</template>
<script>
export default {};
</script>

<style lang="scss" scoped>
.login {
    text-align: center;
}
.logo {
    padding-top: 25%;
    img {
        width: 20%;
        height: 20%;
    }
}
.select {
    padding: 20% 0 0;
    div {
        height: 2rem;
        line-height: 2rem;
        border: 1px solid red;
        border-radius: 5%/50%;
        margin: 5% 10%;
        a {
            text-decoration: none;
            color: red;
        }
        &:last-child {
            color: gray;
            border: 0;
            a {
                color: gray;
                text-decoration: none;
                span {
                    border-bottom: 1px solid gray;
                    font-size: 0.8rem;
                }
            }
        }
    }
}
.other {
    padding-top: 35%;
    width: 100%;
    > div:first-child {
        text-align: center;
        color: gray;
        margin-bottom: 5%;
        font-size: 0.8rem;
    }
    .other-list {
        display: flex;
        justify-content: center;
        align-items: center;
        .other-item img {
            width: 30%;
        }
    }
}
</style>
