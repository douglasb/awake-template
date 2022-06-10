<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="There is no such thing as ready. There is only now."
      subtitle="~ some dude"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h1>prsOldGuy</h1>
          <p>After 30+ years of working behind a computer, that time has taken a toll on my body and I wanted to get back out and do what I love the most: be outside and compete. They say sitting is the new smoking and I agree.  So I'm taking this out of shape 58 3/4 year old body and getting it into mountain tough and into a better place.</p>
          <p>I am interesting in building a community of Senior PRS competitors (55+) and the challenges we face in competition that younger bodies don't have to navigate. Like knee replacements (6 mos since surgery) and a hip replacement (7 yrs out), etc.</p>
          <p>Born in Canada living in the Carolinas since Jr. High, proud to call the Carolina’s my home for more than 40 years.  I am as southern as a southerner will allow me to be.</p>
          <p>A relative newcomer to the the community, I'm focusing on the following areas:
            <ul>
              <li>Competing as a Senior in PRS club and national matches</li>
              <li>Hunting</li>
              <li>Reloading</li>
              <li>Practical hand gun training.</li>
            </ul>
          </p>
          <!-- p><a href="https://www.precisionrifleseries.com/s/13857/prsoldguy/">Precision Rifle Series Profile</a></p -->
          <p>Reach out to me on <a href="https://www.facebook.com/douglasbrownca">Facebook</a> Send me a DM if you want to connect</p>
          <!-- <quote-card /> -->
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
// import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  }
  // components: { QuoteCard }
}

</script>
