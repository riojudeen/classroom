<template>
    <div>
    
        <div class="card chat-box" id="mychatbox">
            <div class="card-header">
            <h3>Forum Diskusi</h3>
            </div>
            <div class="card-body chat-content">
            </div>
            <div class="card-footer chat-form">
            <form id="chat-form">
                <input type="text" class="form-control" placeholder="Type a message">
                <button class="btn btn-primary">
                <i class="far fa-paper-plane"></i>
                </button>
            </form>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            page : "Forum Diskusi"
        }
    },
}
</script>