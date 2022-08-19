<template>
    <div>
        <Post v-for="(user, key) in userList" :key="key" :userData="user"/>

    </div>
</template>

<script>
import Post from './ArticlePost.vue'
export default {
    components:{
        Post,
    },
    props:{
        userList: Object
    }
}
</script>

<style>
</style>