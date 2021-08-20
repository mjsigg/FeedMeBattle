<template>
    <nav>
        <ul class="nav">
                <li><NuxtLink to="/">Home</NuxtLink></li>
                <li><NuxtLink to="/productpage">Product Page</NuxtLink></li>
                <li><NuxtLink to="/producerapplication">Partners</NuxtLink></li>
                <li>Affiliates</li>
        </ul>
    </nav>
</template>

<style>
    nav{
        background-color: aquamarine;
        text-align: center;
        list-style-type: none;
        margin: 0;
        padding: 0;
    }
    nav li{
        display: inline-block;
        padding: 20px;
        font-size: 20px;
    }
    

</style>