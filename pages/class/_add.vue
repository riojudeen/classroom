<template>
    <div>
        <part-pagename :page="page" />
        <div class="card">
            <div class="card-header">
                <h5 class="col-md-10 pl-0">
                    Materi 1
                </h5>
                <div class="col-md-2 text-right pr-0">
                    <button class="btn btn-sm btn-outline-secondary ">
                        <i class="fas fa-arrow-left"></i> 
                    </button>
                </div>
                
                
            </div>
            <div class="card-body">
                <input-type v-for="(sesi, i) in session" :key="i" :name="sesi.name" :type="sesi.type"/>
                <input-type v-for="(start, i) in startDate" :key="i" :name="start.start" :type="start.type"/>
                <input-type v-for="(end, i) in endDate" :key="i" :name="end.end" :type="end.type"/>
                <form action="#" class="dropzone" id="mydropzone">
                    <div class="fallback">
                    <input name="file" type="file" multiple />
                    </div>
                </form>
            </div>
            <div class="card-footer text-right">
                <button class="btn btn-warning">
                    RESET
                </button>
                <button class="btn btn-primary">
                    SAVE
                </button>
            </div>
        </div>
    </div>
    
</template>
<script>
export default {
    data() {
        return {
            page : "Tambah Group Session",
            session: [
                {
                    name : "Nama Session",
                    type : "text",
                }
            ],
            startDate: [
                {
                    start : "Mulai Sesi",
                    type : "date",
                }
            ],
            endDate: [
                {
                    end : "Selesai Sesi",
                    type : "date",
                }
            ],
            
        }
        
    },
    
}
</script>