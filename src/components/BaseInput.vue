<template>
    <div class="my-input">
        <span>
            <slot></slot>
        </span>
        <input v-bind="$attrs"
               :value="value"
               @input="$emit('input', $event.target.value)">
    </div>
</template>

<script>
export default {
    inheritAttrs: false,
    props: ['value']
};
</script>

<style lang="scss" scoped>
.my-input {
    padding-bottom: 1%;
    border-bottom: 1px solid gray;
    margin: 10% 5%;
}
.my-input input {
    border: none;
    outline: none;
    padding-left: 3%;
}
</style>
