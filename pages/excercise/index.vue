<template>
    <div>
        <part-pagename :page="page" />
        <div class="card">
            <div class="card-header">
                <h4>Tugas Mendatang</h4>
            </div>
            <div class="card-body">

            </div>
            <div class="card-footer">
                
            </div>
        </div>
        <div class="card">
            <div class="card-header">
                <h4>Tugas Yang Lalu</h4>
            </div>
            <div class="card-body">

            </div>
            <div class="card-footer">

            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            page : "Excercise"
        }
    },
}
</script>