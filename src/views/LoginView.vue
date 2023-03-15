<template>
    <div class="page">
        <LoginBox @login="$router.push('/home')" />
    </div>
    <div class="page-bg"></div>
</template>
<script>
    import LoginBox from '../components/LoginBox.vue';
    export default{
        data: () => ({

        }),
        components: {
            LoginBox,
        }
    }
</script>
<style scoped>
    .page{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 100vh;
        background-image: url(../assets/logo2.png);
    }
    .page-bg{
        
        filter: blur(8px);
    }
</style>