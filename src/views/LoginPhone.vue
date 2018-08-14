<template>
    <div>
        <BaseHead>手机号登录</BaseHead>
        <!-- <AccountInput :account.sync="account" :password.sync="password"></AccountInput> -->
        <BaseInput maxlength=11
                   type="tel"
                   v-model.number="phone">
            +86
        </BaseInput>
        <BaseInput v-model="password"
                   type="password">
        </BaseInput>
        <BaseButton @click.native="handleLogin">登录</BaseButton>
    </div>
</template>

<script>
import AccountInput from '../components/AccountInput';
export default {
    data() {
        return {
            phone: '',
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
            let params = {
                phone: this.phone,
                password: this.password
            };
            this.$axios.get('/login/cellphone', { params }).then(({ data }) => {
                alert(JSON.stringify(data));
            });
        }
    }
};
</script>

<style lang="scss" scoped>
</style>
