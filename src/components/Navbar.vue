<template>
<nav class="navbar navbar-expand-lg navbar-light bg-orange fixed-top">
    <div class="container">
        <a class="navbar-brand" href="#">
            <img src="https://kozii.id/web/img/logo.png" width="100" height="40" alt="">
        </a> 
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
            <ul class="navbar-nav">
                <li class="nav-item active">
                    <a class="nav-link text-light text-card-small" href="#">Home <span class="sr-only">(current)</span></a>
                </li>
                <li class="nav-item dropdown">
                    <a @click="handleDropdown" class="nav-link dropdown-toggle text-light" href="#" id="navbarDropdownMenuLink" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Product
                    </a>
                    <div class="dropdown-menu">
                        <a class="dropdown-item" v-if="dropdown" href="#">Property</a>
                        <a class="dropdown-item" v-if="dropdown" href="#">Fashion</a>
                        <a class="dropdown-item" v-if="dropdown" href="#">makanan & minuman</a>
                    </div>
                </li>
                <li class="nav-item active">
                    <a class="nav-link text-light" href="#">Blog <span class="sr-only">(current)</span></a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link text-light" href="#">Daftar Member <span class="sr-only">(current)</span></a>
                </li>
                <li class="nav-item active">
                    <a class="nav-link text-light" href="#">Masuk Akun <span class="sr-only">(current)</span></a>
                </li>
            </ul>
        </div>
        <form class="form-inline">
            <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
            <button class="btn btn-warning my-2 my-sm-0" type="submit"><i class="fas fa-search"></i></button>
        </form>
    </div>
</nav>
</template>

<script>
export default {
    data () {
        return {
            dropdown: false
        }
    },
    methods: {
        handleDropdown () {
            if(this.dropdown){
                this.dropdown = false
            }else{
                this.dropdown = true
            }
            console.log(this.dropdown)
        }
    }
}
</script>

<style>
    .bg-orange {
        height: 65px;
        background-color: orangered;    
    } 
    i {
        color: white;
    }  
    a {
        font-size: 14px;
    }
</style>