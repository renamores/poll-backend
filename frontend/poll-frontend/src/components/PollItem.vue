<template>
    <button class="button" @click="goToQuestion(question.id)">
    <div>
        <p>{{question.title}}</p>
    </div>
    </button>
</template>

<script>

export default {
    name: "PollItem",
    props: ["question"],
    methods: {
        goToQuestion(id){
            this.$router.push({name: "question", 
                params:{id: id
                 }
                });
            console.log("go to question");
        }

    }
}
</script>


<style scoped>
.poll-item{
    background: #f4f4f4;
    padding: 10px;
    border-bottom: 1px #ccc dotted;
}

.button{
    background:gray;
    padding: 50px;
    border-bottom: 1px #ccc dotted;
}
</style>