<template>
    <nav>
    <ul>
    <li><router-link to="/">Home</router-link></li>
    <li><router-link to="/about">About</router-link></li>
    <li>{{ 2+2 }}</li>
    </ul>
  </nav>
</template>
<style scoped>
ul li {
    list-style: none;
}
ul {
    display: flex;
    flex-direction: row;
    justify-content: center;
}
</style>
