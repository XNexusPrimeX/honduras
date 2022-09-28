<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
    props: {
        image: {
            type: String,
            required: true,
        },
        author: {
            type: Object
        }
    },
    methods: {
        expandContent() {
            const content = document.querySelector(".content");
            const text = document.querySelector(".text");
            const author = document.querySelector('.author');
            
            content?.classList.toggle("extended");
            text?.classList.toggle("extended");
            author?.classList.toggle("hide");
        }
    }
})
</script>
    
<template>
    <div class="section">
        <div class="images">
            <img :src="`img/${image}`" />
        </div>
        
        <div class="content" v-on:click="expandContent">
            <div class="safeArea">
                <div class="author">
                    <img :src="author.pic" class="pic">
                    <h2 class="name">{{ author.name }}</h2>
                </div>

                <div class="text">
                    <slot />
                </div>
            </div>
        </div>
    </div>
</template>
    
<style scoped>
    .section {
        width: 100vw;
        height: 100vh;
        display: flex;
        flex-direction: row;
    }

    .images {
        z-index: 1;
        overflow: hidden;
        width: 65%;
        height: 100%;
        transition: .3s;
        background-color: black;
    }
    .images img {
        height: 100%;
        object-fit: cover;
        width: 100%;
    }

    .content {
        height: 100%;
        width: 35%;
        display: flex;
        flex-direction: column;
        transition: .3s;
        background-color: rgb(74, 140, 178);
    }
    .content.extended {
        width: 100%;
        transition: .3s;
    }

    .safeArea {
        width: 100%;
        height: 100%;
        margin-top: 120px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .author {
        /* width: 70%; */
        padding: 0 8px;
        height: 60px;
        display: flex;
        align-items: center;
        justify-content: center;
        /* background-color: rgba(255, 255, 255, .1); */
        margin-bottom: 15px;
        border-radius: 50px;
    }
    .author.hide {
        display: none;
    }
    .author img {
        width: 50px;
        height: 50px;
        border-radius: 50px;
        border: 2px solid white;
    }
    .author h2 {
        color: white;
        padding: 0 8px;
        padding-left: 15px;
        font-family: 'Cairo', sans-serif;
        font-weight: lighter;
    }

    .text {
        color: white;
        width: 80%;
        font-style: italic;
        overflow: scroll;
        height: 70vh;
        font-size: 20px;
        border-radius: 10px;
    }
    .text.extended {
        font-size: 250%;
        height: 80vh;
    }
    .text {
        text-indent: 1.5em;
    }
</style>