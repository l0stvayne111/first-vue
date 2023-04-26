<template>
    <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/about">О разработчике</router-link>
    </nav>
    <router-view/>


    <footer>
        All rights reserved.
    </footer>
</template>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;

    min-height: 100vh;
    background: #fff;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

nav {
    padding: 30px;
}

nav a {
    font-weight: bold;
    color: #2c3e50;
    text-decoration: none;
    margin: 0 16px;
}

nav a.router-link-exact-active {
    color: #1e87f0;
}


footer {
    margin-top: auto;
    background: #2c3e50;
    color: #fff;
    text-align: left;
    padding: 32px;
    font-size: 14px;
    font-weight: 400;
}
</style>
