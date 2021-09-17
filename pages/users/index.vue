<template>
    <div>
        <h3>Users route</h3>
        <input type="text" v-model="userId">
        <button @click='findUserById' type="submit">Find User By Id</button>
    </div>
</template>

<script>
export default {
    data(){
        return {
            userId:''
        }
    },
    methods: {
      findUserById() {
        this.$router.push('/users/' + this.userId);
      }  
    },
    layout:'blog'
}
</script>