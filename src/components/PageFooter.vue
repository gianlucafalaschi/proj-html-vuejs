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
            <div class="ms-row py-5 d-flex gap-2">
                <!-- column About -->
                <div class="ms-col-4">
                    <h4 class="ms-col-title">ABOUT</h4>
                    <p class="ms-col-description">Masterstudy is education WordPress theme featured by Learning Management System (LMS) for online education.<br>Developed by StylemixThemes</p>
                    <div class="ms-socials-container d-flex gap-3 fs-4">
                        <i class="fa-brands fa-facebook"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>
                <!-- column Contact -->
                <div class="ms-col-4">
                    <h4 class="ms-col-title">CONTACT</h4>
                    <div class="ms-col-description">
                       <address>
                            <div class="ms-address mb-2">USA, California 20, First Avenue, California</div>
                            <div class="ms-phone">Tel.:+1 212 458 300 32</div>
                            <div class="ms-phone mb-2">FAX.: +1 212 375 24 14</div>
                            <div class="ms-email">info@masterstudy.com</div>
                       </address>
                    </div>
                </div>
                <!-- column Pages -->
                <div class="ms-col-4">
                    <h4 class="ms-col-title">PAGES</h4>
                    <ul class="ms-maps d-flex flex-column gap-1">
                        <!-- dopo aver passato con le props le informazioni presenti in App.vue dell'array footerLinks  all'array footerLinksInfos 
                    per ogni elemento  in  footerLinksInfos stampo-->
                        <li class="ms-pages-links" v-for="footerLinkInfo in footerLinksInfos"><a href="#">{{footerLinkInfo.text}}</a></li>
                    </ul>
                </div>
                <!-- column Blog -->
                <div class="ms-col-4">
                    <!-- single blogs -->
                    <h4 class="ms-col-title">BLOG</h4>
                    <!-- dopo aver passato con le props le informazioni presenti in App.vue dell'array footerBlog  all'array blogInfos 
                    per ogni elemento  in  blogInfo stampo-->
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
    
    width: calc(100% / 4 - 1rem);
    color: $color-third;
    word-wrap: break-word;
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

/* blog */
.ms-row {
    flex-wrap: wrap;
}

.ms-blog-description {

    .ms-blog-date {
        color:$color-fourth;
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
