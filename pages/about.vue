<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Us"
      subtitle="Example About Page"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Fake Heading</h3>
          <p>
            <strong>
              Edit this page in<code>/pages/about.vue</code>to fit your needs.
            </strong>
          </p>
          <p>
            We are two curious humans on a journey to explore the wild west that 
            is Immersive Technology (otherwise known as the XR industry). Through 
            virtual reality, augmented reality, mixed reality and more, immersive 
            technologies are transforming the human experience. Where did it all 
            begin? How far have we come, and how will we tackle the many challenges 
            ahead? We are on a mission to better understand the technology, research, 
            theories and humans behind this fascinating and world-changing industry.  
            We'll talk with people from many walks of life who are helping shape our 
            collective future and explore this emerging reality together. Through 
            deep conversations with these pioneers, we hope to inspire innovation and 
            spread awareness and education so that we may build a more enlightened 
            and equitable future. 
          </p>

          <h3>Another Fake Heading</h3>
          <p>
            We can't do this alone! What began as a passion project will ultimately 
            need support from the community and our listeners to continue and grow.  
            We have a lot of ideas and an ever-growing list of people we'd love to 
            bring on for this season. Your support in making this endeavor a 
            reality(pun intended). Any amount is helpful!
          </p>
          <quote-card />
          <!-- <h3>Still More Fake Content</h3> -->
          <p>
            Whether you can donate or not, we hope you'll be a part of this community. 
            Subscribe, love us, like us, and stay in touch! We would love to hear from 
            you - what you like, what you don't like, who you want us to have on as a 
            guest - whatever it is - you can find our contact info below. 
          </p>
        </div>

        <!-- <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Cool Stuff We Do
              </p>
              <p class="subtitle">
                Sooo Cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Other Cool Things
              </p>
              <p class="subtitle">
                Just as cool
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                All the cool
              </p>
              <p class="subtitle">
                that is all
              </p>
              <figure class="image is-1by1">
                <opti-image width="500" height="500" />
              </figure>
            </article>
          </div>
        </div> -->
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
