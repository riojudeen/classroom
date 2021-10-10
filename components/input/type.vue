<template>
   
        <div class="form-group row">
            <label class="col-md-3 col-form-label" for="">{{name}}</label>
            <div class="col-md-9">
                <input :type="type" :placeholder="'Masukan '+name" class="form-control" v-model="val" >
                <!-- {{value}} -->
            </div>
            
        </div>
</template>
<script>
export default {
    props: {
        name: {
            type: String,
            default: "input",
        },
        value: { type: String, default: "" },
        type: { type: String, default: "text" },
    },
    computed: {
        val: {
            get() {
                return this.value;
            },
            set(value) {
                this.$emit("get", value);
            },
        },
    },
    // methods: {
    //     editValue(value){
    //         // console.log(value);
    //         this.$emit("get", value);
    //     }
    // },
}
</script>