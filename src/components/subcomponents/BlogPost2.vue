<script>
    export default {
        // Add code if/as necessary
        // Hint: Add properties subject, entry and mood
        props: {
            subject: String,
            entry: String,
            mood: String,
        }
    }
</script>


<template>
    <!-- TODO: add your template code here Use boostrap card --> 
    <div class="card">
        <img :src="'../../public/assets/' + mood.toLowerCase() + '.png'">
        <div class="card-header">
            {{subject}}
        </div>
        <div class="card-body">
            <p>{{entry}}</p>
        </div>
        <slot name="delete"></slot>
    </div>
</template>

