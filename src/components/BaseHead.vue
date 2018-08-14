<template>
    <header class="head">
        <router-link to="login">
            <div class="arrow-left">
            </div>
        </router-link>
        <span>
            <slot></slot>
        </span>
    </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.head {
    background-color: red;
    height: 3rem;
    line-height: 3rem;
    color: #ffffff;
}
.arrow-left {
    margin-left: 5%;
    display: inline-block;
    width: 0.7rem;
    height: 0.7rem;
    border-top: 2px solid #ffffff;
    border-right: 2px solid #ffffff;
    transform: rotate(180+45deg);
}
.head span {
    margin-left: 3%;
}
</style>
