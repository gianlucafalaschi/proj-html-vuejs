<script>

</script>

<template>
    <section class="ms-reviews">
        <div class="ms-container-50">
            <div class="ms-row py-5 d-flex flex-column align-items-center">
                <h2 class="text-center mb-4">What Students Say</h2>
                <!-- reviews images -->
                <div class="ms-reviews-images w-100 d-flex justify-content-between  align-items-center mb-3">
                    <span><i class="fa-solid fa-arrow-left-long ms-5"></i></span>
                    <div class="ms-rounds d-flex align-items-center gap-3">
                        <div class="ms-round-container-small rounded-circle overflow-hidden">
                            <img class="img-fluid" src="../assets/img/4-100x100.jpg" alt="">
                        </div>
                        <div class="ms-round-container-big rounded-circle overflow-hidden">
                            <img class="img-fluid" src="../assets/img/2-100x100.jpg" alt="">
                        </div>
                        <div class="ms-round-container-small rounded-circle overflow-hidden">
                            <img class="img-fluid" src="../assets/img/1-100x100.jpg" alt="">
                        </div>
                    </div>
                    <span><i class="fa-solid fa-arrow-right-long me-5"></i></span>
                </div>
                <!-- reviews images -->
                <h5 class="ms-review-title">Paints of the Future</h5>
                <div class="ms-review-stars">
                    <!-- stampare 5 stelle -->
                    <i v-for="n in 5" class="fa-solid fa-star"></i>
                </div>
                <p class="ms-review-text mt-4 text-center">The response to your MaterStudy has been really overwhelming! Those who partecipated in the workshop are spreading the word here on campus and the "buzz" is on. The VP of instruction wants you to come back! Her goal is to have more faculty trained. She also wants to attend a workshop herself. Our president told me MasterStudy needs to be the cornerstone of our success program.</p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;


section {
    background-color: $color-first;
}

.ms-container-50 {
    width: 50%;
    margin: 0 auto;
    padding-left: 10px;
    padding-right: 10px;
}

.ms-round-container-big {
    width: 80px;
    height: 80px;
    background-color: pink;


}

.ms-round-container-small {
    width: 60px;
    height: 60px;
    background-color: coral;


}

.ms-review-stars {
    color: #F2B91E;
}
</style>