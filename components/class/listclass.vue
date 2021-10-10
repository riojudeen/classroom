<template>
    <div>
        <class-modaldetail />
        <div class="card">
            <img :src="img" :alt="name" class="card-img-top">
            <div class="card-body">
                <h5 class="card-title">{{name}}</h5>
                <p class="card-text">{{desc}}</p>
            </div>
            <div class="card-footer row">
                <div class="col-md-6 pull-left">
                    <button class="btn btn-sm btn-outline-primary pull-right " data-toggle="modal" data-target="#exampleModal" >lihat kelas</button>
                </div>
                <div class="col-md-6 text-right">
                    <button-add />
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        id: {
            type: Number,
        },
        name : {
            type: String, //tipe data properti
            default : "Nama Kelas" //default value jika tidak ada inputan
        },
        desc: {
            type: String,
            default : "Deskripsi kelas"
        },
        img: {
            type: String,
            default : "/assets/img/example-image.jpg",
        },
        unfollow: {
            type: Boolean,
            default: false,
        }
    },
}
</script>