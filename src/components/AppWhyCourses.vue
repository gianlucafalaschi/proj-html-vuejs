<script>

</script>


<template>
    <section>
        <div class="ms-container-80">
            <div class="ms-row text-center">
                <h2 class="py-4 mb-0">Why my Courses</h2>
            </div>
            <div class="ms-row d-flex flex-wrap pb-5">
                <!-- card 1 -->
                <div class="ms-card d-flex py-4 px-3">
                    <div class="ms-card-icon me-3">
                        <i class="fa-solid fa-briefcase"></i>
                    </div>
                    <div class="ms-card-description">
                        <h4 class="ms-card-title  pb-3 mb-0">Entrapreneurship</h4>
                        <p class="ms-card-subtitle pb-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Possimus assumenda, aut veniam corrupti fugit, a quibusdam reprehenderit suscipit nesciunt quidem consequatur voluptatum laudantium excepturi ipsam accusamus neque consequuntur! Dolor, quisquam.</p>
                    </div>
                </div>
                <!--/ card 1 -->
                
                <!-- card 2 -->
                <div class="ms-card d-flex py-4 px-3">
                    <div class="ms-card-icon me-3">
                        <i class="fa-solid fa-rocket"></i>
                    </div>
                    <div class="ms-card-description">
                        <h4 class="ms-card-title  pb-3 mb-0">Accelerated learning</h4>
                        <p class="ms-card-subtitle pb-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Possimus assumenda, aut veniam corrupti fugit, a quibusdam reprehenderit suscipit nesciunt quidem consequatur voluptatum laudantium excepturi ipsam accusamus neque consequuntur! Dolor, quisquam.</p>
                    </div>
                </div>
                <!--/ card 2 -->
                <!-- card 3 -->
                <div class="ms-card d-flex py-4 px-3">
                    <div class="ms-card-icon me-3">
                        <i class="fa-regular fa-thumbs-up"></i>
                    </div>
                    <div class="ms-card-description">
                        <h4 class="ms-card-title  pb-3 mb-0">Productivity</h4>
                        <p class="ms-card-subtitle pb-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Possimus assumenda, aut veniam corrupti fugit, a quibusdam reprehenderit suscipit nesciunt quidem consequatur voluptatum laudantium excepturi ipsam accusamus neque consequuntur! Dolor, quisquam.</p>
                    </div>
                </div>
                <!--/ card 3 -->
                <!-- card 4 -->
                <div class="ms-card d-flex py-4 px-3">
                    <div class="ms-card-icon me-3">
                        <i class="fa-solid fa-gear"></i>
                    </div>
                    <div class="ms-card-description">
                        <h4 class="ms-card-title  pb-3 mb-0">Life Coaching</h4>
                        <p class="ms-card-subtitle pb-3">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Possimus assumenda, aut veniam corrupti fugit, a quibusdam reprehenderit suscipit nesciunt quidem consequatur voluptatum laudantium excepturi ipsam accusamus neque consequuntur! Dolor, quisquam.</p>
                    </div>
                </div>
                <!--/ card 4 -->
            </div>
        </div>

    </section>

</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;

section {
    background-color: $color-fifth;
}

.ms-card {
    width: calc((100% / 2) - 24px);
    margin-left: 12px;
    margin-right: 12px;
    margin-top:12px;
    margin-bottom:12px;
    background-color: $color-first;
    border-left: 3px solid $color-second;
    box-shadow: 5px 10px 18px $color-sixth;
}

.ms-card:hover {
    background-color:$color-second ;
    
    .ms-card-icon {
        color: white;
    }

    .ms-card-title {
        color: black;
    }
    .ms-card-subtitle {
        color: black;
    }
}   

.ms-image-container {
    width: 100%;

}


.ms-card-subtitle {
    color: $color-sixth;
}

.ms-card-icon {
    color: $color-second;
    font-size: 35px;
}

.ms-button {
    color:$color-first;
    background-color: $color-second;
    border: none;
    border-radius: 20px;
    padding: 6px 10px;
    font-weight: bold;
    font-size: 14px;
}
</style>
