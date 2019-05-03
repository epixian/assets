<template>
    <div>
        <h1 class="font-normal font-3xl text-grey-darkest leading-none mb-8">
            Site Stats
        </h1>

        <ul>
            <li>
                <strong>Total series</strong>: {{ series }}
            </li>
            <li>
                <strong>Total lessons</strong>: {{ lessons }}
            </li>
        </ul>    
    </div>

</template>

<script>
export default {
    data() {
        return {
            series: 0,
            lessons: 0
        };
    },

    created() {
        axios.get('http://snowman.test:8001/api/stats')
            .then(response => {
                this.series = response.data.series,
                this.lessons = response.data.lessons
            });
    }
};
</script>
