<template>
   <div class="card">
        <div class="card-body">
            <h4 class="card-title">{{ title }}</h4>
            <p class="card-text project-number">
            {{ number }}
            <span>{{ description }}</span>
            </p>
            <span class="card-data">{{ data }}</span>
        </div>
   </div>

</template>

<script>
     export default {
        name: 'Card',
        props: {
            title: String,
            number: String,
            description: String,
            data: String
        }    
    }
</script>

<style scoped>
.card-title {
    font-size: .8em
}
.project-number {
    font-size: 3em;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.project-number span {
    font-size: .35em;
    padding-bottom: 2em;
}

.card-data {
    display: flex;
    justify-content: center;
    padding: .5em 0;
}
</style>
