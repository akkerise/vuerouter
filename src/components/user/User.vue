<template>
    <div>
        <h1>User Component</h1>
        <hr>
        <button @click="navigateHome" class="btn btn-primary">BACK TO HOME PAGE</button>
        <router-view></router-view>
    </div>
</template>

<script type="text/javascript">
    export default {
        methods: {
            navigateHome(){
                this.$router.push('/')
            }
        }
    }
</script>