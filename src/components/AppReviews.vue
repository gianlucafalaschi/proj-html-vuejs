<script>

</script>

<template>
    <section class="ms-reviews">
        <div class="ms-container-50">
            <div class="ms-row py-5">
                <h2 class="text-center mb-4">What Students Say</h2>
                <div class="ms-reviews-images d-flex justify-content-center align-items-center gap-3">
                    <div class="round-container-small rounded-circle">
                        <img src="" alt="">
                    </div>
                    <div class="round-container-big rounded-circle">
                        <img src="" alt="">
                    </div>
                    <div class="round-container-small rounded-circle">
                        <img src="" alt="">
                    </div>
                </div>
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
    border: 1px dashed  black;
}

.round-container-big {
    width: 80px;
    height: 80px;
    background-color: pink;
    
    
}
.round-container-small {
    width: 60px;
    height: 60px;
    background-color: coral;
    
    
}

</style>