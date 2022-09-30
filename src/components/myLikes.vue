<template>
    <p>Click on the likes button below:</p><br>
    <button v-on:click="like()">
        <span v-if="likes >0">{{likes}}</span>
        Like<span v-if="likes > 1 ">s</span> 👍</button>
</template>

<script>
export default {

    data() {
        return {
            likes: 0,
        }
    },
    methods: {
        like() {
            this.likes++;
        }
    }
}
</script>