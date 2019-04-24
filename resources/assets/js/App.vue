<template>
    <div>
        <h1>Vue Router Demo App</h1>
        <p>
            <router-link :to="{ name: 'Test' }">Home</router-link> |
            <router-link :to="{ name: 'About' }">Hello World</router-link>
        </p>


        <div class="container">
            <router-view></router-view>
        </div>
    </div>
</template>

<style>
body{
background-color: white;
};
</style>

<script>
    export default {}
</script>
