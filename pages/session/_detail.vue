<template>
    <div>
        <part-pagename :page="page" />
        
        <material-materi />
    </div>
    
</template>
<script>
export default {
    data() {
        return {
            page : "Sesion 2 : ",
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