<template>
    <div class="carousel-container">
        <b-carousel
            id="carousel-1"
            v-model="slide"
            :interval="4000"
            controls
            indicators
            background="#ababab"
            img-width="650"
            img-height="450"
            style="text-shadow: 1px 1px 2px #333"
        >
            <!--
            It's important that the images here are 13x9 aspect ratio,
            otherwise the page will jump around when the carousel changes.
            -->
            <a href="https://docs.galaxyproject.org/en/master/releases/23.2_announce_user.html" target="_blank">
                <b-carousel-slide
                    img-src="/images/NewToGalaxy.jpeg"
                    img-alt="Galaxy 23.2 is live! A few updates and new features to highlight include new Workflow Comments, the integration of InvenioRDM, and improvements to Workflow Sharing."
                ></b-carousel-slide>
            </a>
            <a href="https://jxtxfoundation.org/news/2024-2-19-gcc/" target="_blank">
                <b-carousel-slide
                    img-src="/images/events/gcc2024/jxtx-gcc2024-fellowships.png"
                    img-alt="JXTX Foundation fellowships available for participating in GCC2024."
                ></b-carousel-slide>
            </a>
            <a href="https://www.biorxiv.org/content/10.1101/2023.06.28.546576v1.full" target="_blank">
                <b-carousel-slide
                    img-src="/images/Paper_Alert_August2023.jpg"
                    img-alt="New paper in preprint titled *Scalable, accessible, and reproducible reference genome assembly and evaluation in Galaxy* by Larivière et al. 2023. Click to read!"
                ></b-carousel-slide>
            </a>
            <a href="https://galaxyproject.org/projects/vgp/" target="_blank">
                <b-carousel-slide
                    img-src="/images/vgp/VGP_hub.jpg"
                    img-alt="The Vertebrate Genomes Project (VGP) is an international collaborative effort by the G10K consortium to generate near error-free genome assemblies for more than 70,000 vertebrate species. Using Galaxy infrasctructure and public instances, this collaboration has generated new, more open methods of genome assembly and access to data."
                ></b-carousel-slide>
            </a>
            <a href="https://jxtxfoundation.org" target="_blank">
                <b-carousel-slide
                    img-src="/images/jxtx/jxtx-jumbotron.png"
                    img-alt="Donate to the James P. Taylor Foundation for Open Science"
                ></b-carousel-slide>
            </a>
            <a href="https://galaxyp.org/" target="_blank">
                <b-carousel-slide
                    img-src="/images/ColabFold_comingsoon.jpeg"
                    img-alt="ColabFold, a machine-learning model based on AlphaFold that is used for predicting the structure of proteins only using only a protein sequence as an input, will soon be available on Galaxy."
                ></b-carousel-slide>
            </a>
        </b-carousel>
    </div>
</template>

<script>
export default {
    name: "Carousel",
    data() {
        return {
            slide: 0,
        };
    },
};
</script>
<style lang="scss" scoped>
.carousel-container {
    padding-top: 2rem;
    max-width: 650px;
    margin: 0 auto;
}
</style>
