<template>
    <div>
        <div class="headerContainer"></div>
        <div class="contentContainerTop"></div>
            <h1>Content Top</h1>
        <div class="contentContainerMiddle"></div>
            <h1>Content Middle</h1>
        <div class="contentContainerBottom"></div>
            <h1>Content Bottom</h1>
    </div>
</template>

<script>
export default {
    data() {
        return {
            contactName: ''
        }
    }
    
}
</script>

<style>

.headerContainer {
    width: 100%;
    background-color: black;
}

.contentContainerTop {
    width: 100%;
    background-color: brown;
}

.contentContainerMiddle {
    width: 100%;
    background-color: yellow;
}

.contentContainerBottom {
    width: 100%;
    background-color: purple;
}

</style>