<template>
    <div>
        <h1>Edit User {{ $route.params.id }}</h1>
    </div>
</template>
<script type="text/javascript">
    export default {
        created() {
            console.log(this.$route.params);
            console.log(this);
        },
        data(){
            return {
                id: this.$route.params.id
            }
        }
    }
</script>