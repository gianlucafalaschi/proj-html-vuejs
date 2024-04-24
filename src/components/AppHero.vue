<script>

</script>


<template>
    <section class="start-revolution">
        <div class="ms-container-80">
            <div class="ms-row d-flex justify-content-end">
                <div class="ms-col-50 ms-col-50-right mt-5">
                    <h1 class="mb-3">Start your Human <span>Revolution</span> today</h1>
                    <p>A wonderful serenity has taken possession of my entire soul, like these sweet mornings of spring which I enjoy with my whole heart.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;


section.start-revolution {
    width: 100%;
    height: 500px;
    background-image:url('../assets/img/slide-1.jpg');
    background-position: top right;
    background-size: cover;
    
}

.ms-col-50-right{
        background-color: transparent;
    }

h1 {
    span {
    color: $color-second;
}
}



</style>

