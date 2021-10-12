<template>
    <div class="main-sidebar">
    <aside id="sidebar-wrapper">
        <div class="sidebar-brand">
        <a href="index.html">ClassRooms</a>
        </div>
        <div class="sidebar-brand sidebar-brand-sm">
        <a href="index.html">CR</a>
        </div>
        <ul class="sidebar-menu">
            <li class="menu-header">Dashboard</li>
            <li class="nav-item dropdown">
            <a href="#" class="nav-link has-dropdown"><i class="fas fa-fire"></i><span>Dashboard</span></a>
            <ul class="dropdown-menu">
                <li><a class="nav-link" href="index-0.html">Presensi</a></li>
                <li><a class="nav-link" href="index.html">Nilai Tugas</a></li>
            </ul>
            </li>
            <li class="menu-header">Kelas</li>
            <li class="active">
                <nuxt-link :to="menu1.to" class="nav-link" ><i :class="menu1.icon"></i> <span>{{menu1.name}}</span></nuxt-link> 
            </li>
            <li class="nav-item dropdown">
            <a href="#" class="nav-link has-dropdown" data-toggle="dropdown"><i class="fas fa-columns"></i> <span>Kelas Saya</span></a>
            <ul class="dropdown-menu">
                <li v-for="(menu, i) in daftarmenu" :key="i" >
                    <nuxt-link :to="menu.to">{{menu.name}}</nuxt-link>
                </li>
                
                
            </ul>
            </li>
           <li class="active">
                <nuxt-link :to="menu2.to" class="nav-link" ><i :class="menu2.icon"></i> <span>{{menu2.name}}</span></nuxt-link> 
            </li>
        </ul>
    </aside>
    </div>
</template>
<script>
export default {
    data() {
        return {
            menu1 : {
                name : "Semua Kelas",
                to : "/class",
                icon : "far fa-square",
            },
            menu2 : {
                name : "Open Library",
                to : "/libs",
                icon : "far fa-square",
            },
            daftarmenu : [
                {  
                    name : "Kelas yang diikuti",
                    to : "/class/myclass",
                },
                {  
                    name : "Presensi",
                    to : "/presensi",
                }
            ]
        }
    },
}
</script>