<template>
    <section class="bg-light" id="portfolio">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-center">
            <h2 class="section-heading text-uppercase">Project</h2>
            <h3 class="section-subheading text-muted">Mini Poyek Yang Pernah Dibuat</h3>
          </div>
        </div>
        <div class="row">
          
            <div class="col-md-4 col-sm-6 project-item" v-for="(obj, key) in projectJSON" :key="key">
                <a class="portfolio-link" data-toggle="modal" href="#portfolioModal2">
                    <div class="portfolio-hover">
                        <div class="portfolio-hover-content">
                            <i class="fas fa-plus fa-3x"></i>
                        </div>
                    </div>
                    <img class="img-fluid" src="img/portfolio/02-thumbnail.jpg" alt="">
                </a>
                <div class="project-caption">
                    <h4>{{ obj.caption }}</h4>
                    <p class="text-muted">{{ obj.title }}</p>
                </div>
            </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    data: () => ({
        projectJSON: [
            {
                img: '/something/random/img.jpg',
                caption: 'Portofolio',
                title: 'Membuat Web Portofolio HTML CSS dan JS'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Tugas Akhir Dicoding Dasar Front-End',
                title: 'Membuat WEB yang memenuhi Semantic web'
            },
            {
                img: '/something/random/img.jpg',
                caption: 'Halaman Login',
                title: 'Membuat Halaman Login belajar dari Youtube menggunakan HTML dan CSS'
            }
        ]
    })
}
</script>

<style lang="css">

</style>


