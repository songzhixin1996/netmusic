<template>
    <div>
        <button>{{value}}</button>
    </div>
</template>

<script>
export default {
    props: ['value']
};
</script>

<style lang="scss" scoped>
div {
    padding: 0 5%;
}
button {
    background-color: red;
    color: white;
    padding: 10px 20px;
    width: 100%;
    text-align: center;
    text-decoration: none;
    display: block;
    font-size: 1rem;
    border: 1px solid red;
    border-radius: 5%/50%;
}
</style>


