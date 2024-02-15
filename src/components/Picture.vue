<template>
    <div>
        <img :src="url" :alt="alt">
    </div>
</template>
<script>
export default {
    name: 'Picture',
    data() {
        return {
            url: '/img/avatar.png',
            alt: 'Avatar'
        }
    }
}
</script>