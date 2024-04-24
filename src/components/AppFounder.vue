<script>

</script>


<template>
    <section class="founder">
        <!-- LIMITED OFFER  -->
        <div class="ms-container-85">
            <div class="ms-row ms-row-offers d-flex rounded-2 ">
                <!-- left col -->
                <div class="ms-col-50  ms-col-50-offer-left p-4">
                    <div class="ms-title-offer mb-3">
                        <h4><span class="text-white">Limited Sale:</span> <span>All courses with 55% off</span></h4>
                    </div>
                    <div class="ms-input">
                        <input class="input-email" type="email" placeholder="Enter your email">
                        <button class="ms-button" type="button">SUBSCRIBE</button>
                    </div>
                </div>
                <!-- right col -->
                <div class="ms-col-50 ms-col-50-offer-right d-flex flex-wrap align-items-center gap-4 p-4">
                    <div class="ms-time-container">
                        <div class="text-center text-white fw-bold fs-1">26</div>
                        <div class="text-center fw-bold">Days</div>
                    </div>
                    <div class="ms-time-container">
                        <div class="text-center text-white fw-bold fs-1">01</div>
                        <div class="text-center fw-bold">Hours</div>
                    </div>
                    <div class="ms-time-container">
                        <div class="text-center text-white fw-bold fs-1">47</div>
                        <div class="text-center fw-bold">Minutes</div>
                    </div>
                    <div class="ms-time-container">
                        <div class="text-center text-white fw-bold fs-1">31</div>
                        <div class="text-center fw-bold">Seconds</div>
                    </div>
                </div>
            </div>
        </div>
        <!--/ LIMITED OFFER  -->
        <!-- FOUNDER DECLARATION -->
        <div class="ms-container-80">
            <div class="ms-row d-flex my-5">
                <!-- left col -->
                <div class="ms-col-50 ms-col-50-left my-5 pe-5">
                    <h3>Hey there, my name is John Doe. I'm the founder of the Brain Academy</h3>
                    <div class="signature-image-container mt-4 d-flex justify-content-center">
                        <img src="../assets/img/sign.jpg" alt="founder's signature">
                    </div>
                </div>
                <!-- right col -->
                <div class="ms-col-50 ms-col-50-right my-5">
                    <p>A wonderful serenity has taken possession of my entire soul, like these sweet mornings of spring
                        which I enjoy with my whole heart. I am alone, and feel the charm of existence in this spot,
                        which was created for the bliss of souls like mine. I am so happy, my dear friend, so absorbed
                        in the exquisite sense of mere tranquil existence, that I neglect my talents. I should be
                        incapable of drawing a single stroke at the present moment; and yet I feel that I never was a
                        greater artist than now. When, while the lovely valley teems with vapour around me, and the
                        meridian sun strikes the upper surface of the impenetrable foliage of my trees, and but a few
                        stray gleams steal into the inner sanctuary</p>
                </div>
            </div>
        </div>
        <!--/ FOUNDER DECLARATION -->
    </section>
</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;

section {
    background-color: $color-first;
    position: relative;
}

.ms-container-85 {
    background-color: pink;
    width: 85%;
    margin: 0 auto;
    padding-left: 10px;
    padding-right: 10px;
    position: absolute;
    left: 50%;
    transform: translate(-50%, -70%);

}

.ms-row-offers {
    background-color: $color-second;
}

.ms-input {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    position: relative;
}

.input-email {
    border-radius: 20px;
    border: none;
    width: 80%;
    font-size: 14px;
    padding: 6px 8px;
}

.ms-button {
    border-radius: 20px;
    border: none;
    position: absolute;
    left: 80%;
    transform: translate(-50%);
    font-size: 14px;
    padding: 6px 8px;
    color: white;
    background-color: $color-third;
}


</style>
