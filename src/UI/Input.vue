<script>
    export default{
        props:{
            placehold: String,
            model: String
        },
        methods: {
        updatePropValue(event) {
        this.$emit('update:model', event.target.value);
        }
  }
    }
</script>

<template>
    <input :placeholder ="placehold" :model ="model" @input="updatePropValue"/>
</template>

<style>
    input{
        border-radius: 46px;
        border: 1px solid var(--Neutral-300, #EFF0F6);
        background: var(--Neutral-100, #FFF);
        /* Input/Default */
        box-shadow: 0px 2px 6px 0px rgba(19, 18, 66, 0.07);

        height: 66px;
        width: 284px;
        padding-left: 20px;

        color: var(--Neutral-600, #6F6C90);
        /* Other/18-20 R */
        font-family: "DM Sans";
        font-size: 18px;
        font-style: normal;
        font-weight: 400;
        line-height: 20px; /* 111.111% */
    }
</style>