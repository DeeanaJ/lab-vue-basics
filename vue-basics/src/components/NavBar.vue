<template>
    <nav>
        <ul>
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/about">About</router-link></li>
            <li>{{ 2+2 }}</li>
        </ul>
     </nav>
     <button @click="awesome = !awesome">Mis nombres</button>

    <h1 v-if="awesome">Diana</h1>
    <h1 v-else>Roxana</h1>
</template>
<script>
export default {
  data() {
    return {
      awesome: 0,
    };
  },
};
</script>
<style scoped>
ul li {
    list-style: none;
}
ul {
    display: flex;
    flex-direction: row;
    justify-content: center;
}

button {
    background-color: #42b983;
    border: none;
    padding: 12px;
    color: #fff;
    border-radius: 8px;
    cursor: pointer;
    font-weight: 600;
}

button:hover {
    background-color: #30a26f;
}

button:active {
    background-color: #228b5c;
}
</style>
