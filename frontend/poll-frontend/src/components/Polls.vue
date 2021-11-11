<template>
    <div>
        <h1>Questions</h1>
        <div v-bind:key ="question.id" v-for="question in questions" >
            <PollItem v-bind:question="question"/>
        </div>
    </div>
</template>

<script>
import PollItem from "./PollItem.vue";

export default {
    name: "Polls",
    components: {
        PollItem
    },
    props: ["questions"]
}
</script>

<style scoped>

</style>