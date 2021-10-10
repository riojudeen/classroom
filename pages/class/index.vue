<template>
    <div class="row">
        <div class="col-md-4" v-for="(kelas, i) in listClass" :key="i" >
            <class-listclass :img="kelas.img" :name="kelas.name" :desc="kelas.desc" />
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            listClass : [
                {
                    name : "Static Web", 
                    desc: "Ini Deskripsi Kelas Fullstack 5",
                    img: "/assets/img/example-image.jpg"
                },
                {name : "GIT", desc: "Ini Deskripsi Kelas Fullstack 6"},
                {name : "Deployment", desc: "Ini Deskripsi Kelas Fullstack 7"},
                {name : "Fundamental", desc: "Ini Deskripsi Kelas Fullstack 8"},
                {name : "Javascript", desc: "Ini Deskripsi Kelas Fullstack 9"},
                {name : "FrontEnd", desc: "Ini Deskripsi Kelas Fullstack 9"},
            ]
        }
    },
}
</script>