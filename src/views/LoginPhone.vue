<template>
    <div>
        <BaseHead>手机号登录</BaseHead>
        <AccountInput :account.sync="account" :password.sync="password"></AccountInput>
        <BaseButton>登录</BaseButton>
    </div>
</template>

<script>
import AccountInput from '../components/AccountInput';
export default {
    data() {
        return {
            account: '',
            password: ''
        };
    },
    components: {
        AccountInput
    },
    methods: {
        storeAccount() {
            this.$store.commit('setAccount', {
                account: this.account,
                password: this.password
            });
        },
        handleLogin() {
            this.storeAccount();
        }
    }
};
</script>

<style lang="scss" scoped>
</style>
