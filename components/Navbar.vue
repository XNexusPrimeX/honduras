<script lang="ts">
import Vue from "vue";

export default Vue.extend({
    name: "Navbar",
});
</script>
    
<template>
    <div class="navbar">
        <div class="background">
            <div class="titles">
                <h1>Honduras</h1>
            </div>
            <ul class="links">
                <router-link to="/picobonito">Pico Bonito</router-link>
                <router-link to="/cochinos">Cochinos</router-link>
                <router-link to="/lagoyojoa">Lago Yojoa</router-link>
                <router-link to="/roatan">Roatán</router-link>
                <router-link to="/utila">Útila</router-link>
            </ul>
        </div>
    </div>
</template>
    
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Cairo:wght@400&family=Gideon+Roman&display=swap");

* {
    color: white;
}
.navbar {
    position: fixed;
    z-index: 2;
    width: 100vw;
    height: 120px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.background.hide {
    position: fixed;
    width: 70px;
    transition: 0.5s;
}
.background {
    width: 90vw;
    height: 70px;

    background-color: rgba(33, 161, 235, 0.4);
    backdrop-filter: blur(15px);
    border-radius: 50px;

    display: flex;
    align-items: center;
    justify-content: space-between;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: 0.3s;
}
.titles {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-left: 10vw;
}
h1 {
    font-size: 35px;
    font-family: "Gideon Roman", cursive;
    text-transform: uppercase;
    /* letter-spacing: 20px; */
}
ul {
    text-decoration: none;
    list-style: none;
    display: flex;
    padding-right: 10vw;
    font-size: 15px;
}
.links a {
    padding: 0 15px;
}
.links a {
    font-family: "Cairo", sans-serif;
    text-transform: uppercase;
    text-decoration: none;

    transition: 1s;
}
.links a:hover {
    transition: 0.2s;
    cursor: pointer;

    text-shadow: 0 0 10px white, 0 0 20px white;
    /* 0 0 30px white; */
}
.links a:active {
    text-shadow: 0 0 10px white, 0 0 20px white, 0 0 30px white, 0 0 40px white;
}
</style>