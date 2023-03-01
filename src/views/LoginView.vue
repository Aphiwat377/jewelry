<script setup>
    import Login from '../components/LoginUI.vue'
    import { RouterLink, RouterView } from 'vue-router'

</script>
<template>
    <main>
        <Login />
        
        <div class="sigh">
        or
        
        <br>
        <RouterLink to="/signin">Sign Up</RouterLink>
        </div>
        

    </main>




<RouterView />
</template>

<style scoped>
.sigh {
  margin-top: 2rem;

}
</style>