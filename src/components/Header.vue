<template>
    <header>
        <h1>{{title}}</h1>
        <Button text="Add Task" color="Green" />
    </header>
</template>

<script>
import Button from './Button'

export default{
    name: 'Header',
    props: {
        title: String,
    },
    components: {
        Button,
    }
}
</script>

<!-- scoped means anything in here is only for this or specific component-->
<style scoped> 
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>