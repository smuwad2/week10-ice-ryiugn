<script>
    // TODO: Complete the code
    export default { 
        data() {
            return {
                
            }
        },
        // Hint: insert properties task (Object) and idx (Number)
        props: {
            task: Object,
            idx: Number
        },
        emits: ['taskDone']
    }
</script>

<template>
    <!-- TODO: add your template code here --> 
   <div class="card">
    <div class="card-title">
        Deadline: {{task.deadline}}
    </div>
    <p class="card-subtitle">
        {{task.desc}}
    </p>
    <button class="btn btn-primary" v-on:click="$emit('taskDone', idx)">Done</button>
   </div>
</template>


