<template>
    <div>
        <h1>{{theTitle}}</h1>
        <p v-for="task in taskList" v-bind:key="task.id">{{task.titel}}</p>
    </div>
</template>

<script>
export default {
    name:"TaskList",
    props:['theTitle', 'taskList']
}
</script>