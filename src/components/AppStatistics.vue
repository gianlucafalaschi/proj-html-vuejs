<script>
</script>

<template>
    <section class="ms-statistics">
        <div class="ms-container-80">
            <div class="ms-row d-flex flex-wrap justify-content-center gap-5">
                <!-- statistic -->
                <div class="ms-one-stats d-flex justify-content-center gap-3 align-items-center">
                    <span class="ms-icon"><i class="fa-solid fa-user-group"></i></span>
                    <div class="ms-stats-info">
                        <div class="ms-stats-numbers fw-bold">1000</div>
                        <div class="ms-stats-description text-white">Online learner</div>
                    </div>
                </div>
                <!--/ statistic -->
                <!-- statistic -->
                <div class="ms-one-stats d-flex justify-content-center gap-3 align-items-center">
                    <span class="ms-icon"><i class="fa-solid fa-film"></i></span>
                    <div class="ms-stats-info">
                        <div class="ms-stats-numbers fw-bold">23</div>
                        <div class="ms-stats-description text-white">Video Courses</div>
                    </div>
                </div>
                <!--/ statistic -->
                <!-- statistic -->
                <div class="ms-one-stats d-flex justify-content-center gap-3 align-items-center">
                    <span class="ms-icon"><i class="fa-regular fa-image"></i></span>
                    <div class="ms-stats-info">
                        <div class="ms-stats-numbers fw-bold">437</div>
                        <div class="ms-stats-description text-white">Sliders & Images</div>
                    </div>
                </div>
                <!--/ statistic -->
                <!-- statistic -->
                <div class="ms-one-stats d-flex justify-content-center gap-3 align-items-center">
                    <span class="ms-icon"><i class="fa-regular fa-thumbs-up"></i></span>
                    <div class="ms-stats-info">
                        <div class="ms-stats-numbers fw-bold">1440</div>
                        <div class="ms-stats-description text-white">Exellent Reviews</div>
                    </div>
                </div>
                <!--/ statistic -->
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;

section.ms-statistics{
    background-image: url('../assets/img/counter-1919x1101.jpg');
    background-size: cover; 
    background-position: 100% 20%;
   
}

.ms-row {
    padding-top: 60px;
    padding-bottom: 60px;
    min-height: 350px;
}

.ms-icon {
    color: white;
    font-size: 35px;
}

.ms-stats-numbers {
    color: $color-second ;
    font-size: 35px;
}

</style>