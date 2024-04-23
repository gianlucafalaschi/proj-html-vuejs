<script>
export default {
    props: {
        headerInfos: Array
    },
}
</script>


<template>
    <header>
        <div class="ms-container-80">
            <div class="ms-row d-flex justify-content-between align-items-center py-4">
                <div class="ms-logo-section d-flex">
                    <img src="../assets/img/MasterStudy-1.svg" alt="">
                </div>
                <div class="ms-links-socials d-flex">
                    <div class="ms-links-section me-4">
                        <nav>
                            <ul class="ms-links d-flex align-items-center mb-0">
                                <li v-for="headerInfo in headerInfos">{{ headerInfo.text }}</li>
                            </ul>
                        </nav>
                    </div>
                    <div class="ms-socials-section d-flex align-items-center ">
                        <ul class="ms-socials-links d-flex align-items-center mb-0">
                            <li><i class="fa-brands fa-facebook"></i></li>
                            <li><i class="fa-brands fa-facebook"></i></li>
                            <li><i class="fa-brands fa-facebook"></i></li>
                            <li><i class="fa-brands fa-facebook"></i></li>
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

.ms-container-80 {
border: 1px dashed black;
  
}

.ms-row {
    border: 1px dashed black;

}

ul.ms-links {
    list-style: none;
    gap: 15px;
}

ul.ms-socials-links {
    list-style: none;
    gap: 10px;
    color: $color-third;
}

</style>