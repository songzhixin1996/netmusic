<template>
    <div class="login">
        <div class="logo">
            <img src="../assets/logo.jpg">
        </div>
        <div class="select">
            <div>手机号登录</div>
            <div>注册</div>
            <div>
                <router-link to="asd">游客登录</router-link>
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
.logo {
    img {
        margin: 10% auto;
        width: 20%;
        height: 20%;
    }
}
.select {
    color: red;
    div {
        height: 2rem;
        line-height: 2rem;
        border: 1px solid red;
        border-radius: 5%/50%;
        margin: 5% 5%;
        &:last-child {
            color: gray;
            border: 0;
            a:visited {
                color: gray;
            }
        }
    }
}
.other {
    position: absolute;
    bottom: 3%;
    width: 100%;
    > div:first-child {
        text-align: center;
        color: gray;
        margin-bottom: 5%;
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
