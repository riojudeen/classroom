<template>
    <section class="section">
        <div class="section-header">
        <h1>{{page}}</h1>
        </div>

        <div class="section-body">
        </div>
    </section>
</template>
<script>
export default {
    props: {
        page : {
            type: String,
            default: "blank"
        }
    }
}
</script>
