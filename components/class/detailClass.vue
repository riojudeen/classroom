<template>
    <div class="card">
        <div class="row no-gutters">
            <div class="col-md-4">
            <img :src="img" >
            </div>
            <div class="col-md-8">
                <div class="card-header">
                    <h4 class="card-title">Session 1 : Materi 1</h4>
                    <div class="card-header-action">
                        <div class="btn-group dropleft">
                            <button type="button" class="btn bg-transparent text-primary" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            <i class="fas fa-ellipsis-v"></i>
                            </button>
                        <div class="dropdown-menu dropleft">
                            <nuxt-link to="../session/1234" class="dropdown-item" ><i class="fas fa-eye"></i> View</nuxt-link>
                            <a class="dropdown-item" href="#"><i class="far fa-edit"></i> Edit</a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#"><i class="far fa-trash-alt"></i> Delete</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="card-body">
                
                
                <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
                <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
            </div>
            </div>
        </div>
    </div>
    
</template>
<script>
export default {
    props: {
        img: {
            type: String,
            default: "assets/img/example-image.jpg",
        }
    }
}
</script>