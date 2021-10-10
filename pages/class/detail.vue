<template>
    <div>
        <head-jumbotron />
        <class-actionclass />
        <class-detailClass />
        <class-actionclass />
        <class-detailClass />
       
    </div>
</template>
<script>
export default {
    data() {
        return {
            part: "class",
            listMateri : [
                {
                    materi : "Materi 1",
                    source : "",
                    img : ""
                }
            ],
        }
    },
}
</script>