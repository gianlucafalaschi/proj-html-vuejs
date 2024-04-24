<script>
export default {
    props: {
        footerLinksInfos: Array,
        blogInfos: Array,
    },
    methods: {
        getImageUrl(name) {
                return new URL(`../assets/img/${name}`, import.meta.url).href;
            }
    }
}
</script>


<template>
    <footer>
        <div class="ms-container-80">
            <div class="ms-row d-flex gap-4">
                <!-- column About -->
                <div class="ms-col-4">
                    <h4 class="ms-col-title">ABOUT</h4>
                    <p class="ms-col-description">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Mollitia,
                        neque id. Minus ad nostrum reprehenderit asperiores, omnis magni aliquid animi numquam beatae,
                        quidem quia non distinctio odit nihil tempora iusto?</p>
                    <div class="ms-socials-container d-flex gap-3">
                        <i class="fa-brands fa-facebook"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>
                <!-- column Contact -->
                <div class="ms-col-4">
                    <h4 class="ms-col-title">ABOUT</h4>
                    <div class="ms-col-description">
                       <address>
                            <div class="ms-address mb-2">Indirizzo</div>
                            <div class="ms-phone">43343433434o</div>
                            <div class="ms-phone mb-2">43343433434o</div>
                            <div class="ms-email">email</div>
                       </address>
                    </div>
                </div>
                <!-- column Pages -->
                <div class="ms-col-4">
                    <h4 class="ms-col-title">Pages</h4>
                    <ul class="ms-maps d-flex flex-wrap gap-5">
                        <li class="ms-pages-links" v-for="footerLinkInfo in footerLinksInfos"><a href="#">{{footerLinkInfo.text}}</a></li>
                    </ul>
                </div>
                <!-- column Blog -->
                <div class="ms-col-4">
                    <!-- single blogs -->
                    <h4 class="ms-col-title">BLOG</h4>
                    <div v-for="singleBlogInfo in blogInfos" class="ms-blog-container d-flex flex-wrap gap-3 mb-3">
                        <div class="ms-image-container">
                            <img :src="getImageUrl(singleBlogInfo.image)" alt="immagine del blog">
                        </div>
                        <div class="ms-blog-description">
                            <h5 class="ms-blog-title">{{singleBlogInfo.title}}</h5>
                            <span class="ms-blog-date">{{'- ' + singleBlogInfo.date}}</span>
                        </div>
                    </div>
                    <!-- /blog -->
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use'../style/partials/_variables' as *;



footer {
    background-color: $color-second ;
}

.ms-col-4 {
    background-color: coral;
    width: calc(100% / 4);
    color: $color-third;

}

.ms-maps {
    list-style-position: outside;
}

li {

    a {
        
        color: $color-third;
        text-decoration:none;
    }
}



.ms-blog-description {

    .ms-blog-date {
        color:$color-sixth;
    }
}

.ms-image-container {
    width: 70px;
    height: 70px;

    img {
        width: 100%;
    }
}

</style>
