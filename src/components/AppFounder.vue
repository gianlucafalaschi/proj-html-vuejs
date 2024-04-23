<script>

</script>


<template>
    <section class="founder">
        <div class="ms-container-85">
            <div class="ms-row ms-row-offers d-flex rounded-2 ">
                <div class="ms-col-50 p-4">
                    <div class="ms-title-offer">
                        <h4>Limited Sale: All courses with 55% off</h4>
                    </div>
                    <div class="ms-input">
                        <input class="input-email" type="email" placeholder="Enter your email">
                        <button class="ms-button" type="button">SUBCRIBE</button>
                    </div>
                </div>
                <div class="ms-col-50 p-4">ciao</div>
            </div>
        </div>
        <div class="ms-container-80">
            <div class="ms-row d-flex my-5">
                <div class="ms-col-50 ms-col-50-left my-5 pe-5">
                    <h3>Hey there, my name is John Doe. I'm the founder of the Brain Academy</h3>
                    <div class="signature-image-container mt-4 d-flex justify-content-center">
                        <img src="../assets/img/sign.jpg" alt="founder's signature">
                    </div>
                </div>
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
    border: 1px dashed black;
    position: absolute;
    left: 50%;
    transform: translate(-50%, -70%);

}

.ms-row-offers {
    border: 1px dashed red;
}

.ms-input {
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    position: relative;
}

.input-email {
    border-radius: 20px;
    width: 80%;
    
}

.ms-button {
    border-radius: 20px;
    position: absolute;
    left: 80%;
    transform: translate(-50%);
}
</style>
