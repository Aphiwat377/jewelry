<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
 
  <header>
    
    <nav>
            
        <RouterLink to="/">Home</RouterLink>
        
      <div class="log">

        <RouterLink to="/profile">Profile</RouterLink>

        
        <RouterLink to="/login">Login / Sig up</RouterLink>

  
      </div>
      </nav>
    <div class="wrapper">

      
      
    </div>


   
      

    
  </header>

  

  <RouterView />
</template>

<style scoped>
.log{
  left: 80%;
  position: fixed;
  display: flex;
  justify-content: space-between;

}

header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  align-items: center;
  
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: block;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  .logo {
    margin: 0 2rem 0 0;
  }
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
