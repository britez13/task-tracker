<template>
    <header>
        <h1>{{ title }}</h1>
        <ButtonComp text="Add task" color="green" />
    </header>
</template>

<script>
    import ButtonComp from "./Button"
    export default {
        name: 'HeaderView',
        props: {
            title: String
        }, 
        components: {
            ButtonComp
        }
    }
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px
    }
</style>