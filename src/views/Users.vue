<template>
    <div>
        <h1>Users</h1>
        <p>this user number is {{ userId }}</p>
        {{ $route.params.name }}
    </div>
</template>

<script>
export default {
    computed: {
        userId() {
            return this.$route.params.userId
        }
    },
    created() {
        console.log("router", this.$router) // info about router.js
        console.log("route", this.$route) // info about this page route
        console.log("test")
    }
}
</script>
