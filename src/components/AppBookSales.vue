<script>

</script>


<template>
    <section class="ms-book-sales">
        <div class="ms-options-box bg-white d-flex flex-column align-items-center py-2 gap-3 text-black">
            <a href="#"><i class="fa-solid fa-desktop"></i></a>
            <a href="#"><i class="fa-regular fa-life-ring"></i></a>
            <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
            <a href="#"><i class="fa-solid fa-desktop"></i></a>
            <a href="#"><i class="fa-solid fa-mobile-screen-button"></i></a>
        </div>
        <div class="ms-container-80">
            <div class="ms-row">
                <div class="ms-col-50 ms-col-50-left text-center d-flex flex-column align-items-center  py-5">
                    <h2 class="ms-title fw-bold">Get my Exclusive Investing Book just for $19.50</h2>
                    <p class="text-white fst-italic">Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident fugit blanditiis beatae consectetur ut? Reiciendis, minima? Itaque consequuntur doloremque dicta quibusdam, repudiandae illo atque harum consequatur, quidem velit eligendi nisi?</p>
                    <div class="ms-amazon-button">
                        <a href="#">
                            <img src="../assets/img/amazon.png" alt="amazon button">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;



section {
    width: 100%;
    background-image:url('../assets/img/slider_1-1917x607-1914x606.jpg');
    background-position: top right;
    background-size: cover;
    position: relative;
    
}

.ms-options-box {
    width: 50px;
    position: absolute;
    right: 0;
    top: 30px;
    

    i {
       color:$color-third ;
        
    }
}

.ms-row {
    display: flex;
    background-image: url('../assets/img/book.png');
    background-size: contain;
    background-repeat: no-repeat;
    background-position:bottom right;
}

.ms-col-50-left {
    .ms-title{
        color: $color-second;
    }
}

.ms-amazon-button {
    width: 150px;
    
    img{
        width: 100%;
    }
}


.ms-col-50-right {
    background-image: url('../assets/img/book.png');
    background-size: contain;
    background-repeat: no-repeat;
    margin-top: 25px
}

</style>

