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
          <h1>About prsOldGuy</h1>
          <p>Born in Canada living in the Carolinas since Jr. High, proud to call the Carolina’s my home for more than 40 years.  I am as southern as a southerner will allow me to be.</p>
          <p>A relative newcomer to the the community, I'm focusing on the following areas:
            <ul>
              <li>Competing as a Senior in PRS club and national matches</li>
              <li>Hunting</li>
              <li>Reloading</li>
              <li>Practical hand gun training.</li>
            </ul>
            <h3>Current Challenges</h3>
            <p>A knee replacement late 2021 has not progressed as would like and I'm still getting used to the new hardware and what it means for position building during PRS matches.</p>
          </p>
          <p><a href="https://www.precisionrifleseries.com/s/13857/prsoldguy/">Precision Rifle Series Profile</a></p>
          <p><a href="https://www.facebook.com/douglasbrownca"></a>Facebook</p>
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
  },
 // components: { QuoteCard }
}
</script>
