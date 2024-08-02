<script>
export default {
    props: {
        headerInfos: Array,
        headerSocials:Array
    },
     data(){
        return {
            activeLink: 0,  // valore standard dell'active link
        }
     },
     methods: {
        /* funzione che assegna al valore di activeLink il valore di index  */
        elementIsActive: function(index){
            this.activeLink = index;
        }
     }
}
</script>


<template>
    <header>
        <div class="ms-container-80">
            <div class="ms-row d-flex justify-content-between align-items-center flex-wrap py-4">
                <div class="ms-logo-section d-flex">
                    <img src="../assets/img/MasterStudy-1.svg" alt="">
                </div>
                <div class="ms-links-socials d-flex flex-wrap">
                    <div class="ms-links-section me-4">
                        <nav>
                            <ul class="ms-links d-flex align-items-center flex-wrap mb-0">
                                <!--  dopo aver passato al'array headerInfos  nelle props di PageHeader l'array headerLinks,
                                Per ogni elemento di nell'array headerInfos,
                                stampo text  -->
                                <!-- al click del mouse sull'elemento li viene richiamata la funzione elementIsActive che
                                assegna il valore dell'index ad activeLink -->
                                <!-- tramite la classe dinamica viene assegnata la classe active all'elemento che che viene cliccato -->
                                <li class="py-3" v-for="headerInfo, index in headerInfos" :class="{'active' : index == activeLink}" @click="elementIsActive(index)">
                                    <a class="fw-bold" href="#">{{ headerInfo.text }}</a>
                                    <span v-if="index == 2" class="badge ms-badge-header text-bg-danger">NEW</span>
                                </li>
                            </ul>
                        </nav>
                    </div>
                    <div class="ms-socials-section d-flex align-items-center ">
                        <ul class="ms-socials-links d-flex align-items-center mb-0">
                            <li class="py-3" v-for="headerSocial in headerSocials"><a href="#"><i :class="headerSocial.social"></i></a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;


header {
    background-color: $color-first;
}

h1 {
    color: $color-second;
}


ul.ms-links {
    list-style: none;
    gap: 15px;
    
    li {
        position: relative;
        border: 3px solid transparent;
        &.active{
            border-bottom: 3px solid $color-second;
        }
    }
    
    
}

.ms-badge-header {
    position: absolute;
    top: 8px;
    left:100%;
    transform: translate(-50%, -50%);
}

ul.ms-socials-links {
    list-style: none;
    gap: 10px;
    color: $color-third;
}

li {
    a {
        text-decoration: none;
        color:$color-third;
    }
    
}


</style>