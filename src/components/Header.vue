<template>
    <header>
        <h1>{{title}}</h1>
        <Button @btn-click="$emit('toggle-add-task')" :text="showAddTask ? 'Close' : 'Add Task'" :color="showAddTask ? 'Red' : 'Green'" />
    </header>
</template>

<script>
import Button from './Button'

export default{
    name: 'Header',
    props: {
        title: String,
        showAddTask: Boolean,
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