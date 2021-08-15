<template>
    <div class="headerContainer">
        <div class="navContainer">
                <NuxtLink to="/"><h1>Home page</h1></NuxtLink>
                <NuxtLink to="/"><h1>About</h1></NuxtLink>
                <NuxtLink to="/"><h1>Partners</h1></NuxtLink>
        </div>

        <div class="alert alert-primary" role="alert">
  This is a primary alert—check it out!
</div>
    </div>
</template>

<style>
.headerContainer {
    width: 100%;
    margin: auto;
    background-color: purple;
}
.navContainer {
    width: 60%;
    background-color: gray;
    margin: auto;
}



</style>