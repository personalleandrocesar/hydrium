<script setup lang="ts">
useHead({
    titleTemplate: 'Hydriun',
})

</script>

<template>

  <Nav/>
  <header>
  
    <div class='logo'>
    
        <h1 class=''>Hydriun</h1>
        <NuxtLink :to="{path:'/', hash: '#websites'}" class="animate">
            <Icon class="arrow" name='ion:md-arrow-down'/>
        </NuxtLink>

    </div>
    
  </header>
  
  <Home/>
  
</template>

<style scoped>

@keyframes clickAnimation {
    0% {
      transform: translateY(-10px);
    }
    50% {
      transform: translateY(10px);
    }
    100% {
      transform: translateY(-10px);
    }
  }

.animate {
  animation: clickAnimation 3s ease infinite;
}

.logo{
margin: 0 auto 80px auto;
  height: 90vh;
  display: flex;
  flex-wrap: nowrap;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  font-family: 'Nirequa';
  color: var(--color-text);
}

.ani {
    
animation: updown 3s ease infinite;
}

.arrow {
  margin-top: auto;
margin-bottom: 64px;
-webkit-animation: updown 3s ease infinite;
animation: updown 3s ease infinite;
height: 60px;
zoom: 0.7;
color: var(--color-detail);
}

h1{
  margin-top: auto;
padding: 0 48px;
    font-size: 3rem;
    margin: 0 auto;
height: 100vh;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
      color: var(--color-detail);
}

h3{
  color: var(--color-text);
  margin-top: -1rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin: 2rem 0 ;
}

nav a {
  color: var(--color-text);
  font-weight: bold;
  font-size: .9rem;
}
nav a:hover {
  color: #33333320;
}

nav a.router-link-exact-active {
  color: #333;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
