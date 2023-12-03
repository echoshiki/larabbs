<script setup>
    import { ref } from 'vue'
    const props = defineProps({
        theme: {
            type: String,
            default: 'flat',
        }
    })
    const url = ref('/captcha/' + props.theme)
    function refresh(){
        url.value = '/captcha/'+ props.theme + '?' + Math.random()
    }
</script>

<template>
    <img :src="url" @click="refresh" title="点击图片重新获取验证码">
</template>