<template>
         <div class="card card-danger">
          <div class="card-header">
            <h4 style="font-size:27px">Materi</h4>
            <div class="card-header-action">
              
              <div class="btn-group dropleft">
                <button type="button" class="btn bg-transparent text-primary" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                <i class="fas fa-ellipsis-v"></i>
                </button>
              <div class="dropdown-menu dropleft">
                <nuxt-link to="add" class="dropdown-item" ><i class="fas fa-plus"></i> Add</nuxt-link>
                <a class="dropdown-item" href="#"><i class="far fa-edit"></i> Edit</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#"><i class="far fa-trash-alt"></i> Delete</a>
              </div>
            </div>
            </div>
          </div>
          
        </div>
</template>