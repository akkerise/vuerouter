<template>
    <div>
        <h1>UserDetail Component</h1>
        <p>Load ID : {{ id }}</p>
        <!--<router-link tag="button" :to="'/user/' + id + '/edit'" class="btn btn-warning">Edit User {{ id }}</router-link>-->
        <router-link tag="button" :to="{name: 'userEdit', params: {id: $route.params.id}}" class="btn btn-warning">Edit User {{ id }}</router-link>
    </div>
</template>

<script type="text/javascript">
    export default {
        data(){
            return {
                id: this.$route.params.id
            }
        }
    }
</script>