<template>
    <div>
        <button :style="sytleObj">
            <slot>确定</slot>
        </button>
    </div>
</template>

<script>
export default {
    props: ['type'],
    computed: {
        sytleObj() {
            let obj;
            if (this.type === 'blank') {
                obj = {
                    backgroundColor: '#fff',
                    color: '#000'
                };
            }
            return obj;
        }
    }
};
</script>

<style lang="scss" scoped>
div {
    padding: 0 5%;
}
button {
    outline: none;
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
    &:active {
        background-color: rgb(163, 56, 56);
    }
}
</style>


