<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Our Team"
      subtitle="Socially responsible"
      image="/uploads/mga-team.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <h3>Founders</h3>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
                <p class="subtitle">
                  <b>Pedro Teixeira - CEO</b>
                </p>
              </div>
              <div id="right" style="float:right">
                <figure class=" ">
                  <opti-image
                    :src="require('~/assets/uploads/Pedro Teixeira.png').src"
                    :srcset="
                      require('~/assets/uploads/Pedro Teixeira.png').srcSet
                    "
                    width="125"
                    height="125"
                  />
                </figure>
              </div>
              <div style="text-align:justify">
                Regional Director in a listed MNC
                <br />
                15+ years in P&L & M&S experience
                <br />
                Lived in Portugal, UK, Doha & Singapore
                <br />
                Master in Engineering; MBA
                <br />
                Top 10 in the Portuguese 40 Under 40 Award
              </div>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
                <p class="subtitle">
                  <b>Bruno Sousa - CTO</b>
                </p>
              </div>
              <div id="right" style="float:right">
                <figure class=" ">
                  <opti-image
                    :src="require('~/assets/uploads/Bruno Sousa.png').src"
                    :srcset="require('~/assets/uploads/Bruno Sousa.png').srcSet"
                    width="125"
                    height="125"
                  />
                </figure>
              </div>
              <div style="text-align:justify">
                IT Manager & Technology Strategist
                <br />
                15+ years experience
                <br />
                Lived in Portugal, France and Switzerland
                <br />
                Engineering Degree in Computing Science; MBA
                <br />
                Team Leader at CERN
              </div>
            </article>
          </div>
        </div>
        <div class="content">
          <h3>MyGreenApp team</h3>
          <div class="tile is-ancestor">
            <div class="tile is-parent">
              <article class="tile is-child box">
                <div id="left">
                  <figure class=" ">
                    <opti-image
                      :src="require('~/assets/uploads/MGA_20210527.png').src"
                      :srcset="
                        require('~/assets/uploads/MGA_20210527.png').srcSet
                      "
                      width="950"
                      height="375"
                    />
                  </figure>
                </div>
              </article>
            </div>
          </div>
        </div>
      </template>
      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest News
        </h3>
        <!-- Latest Posts -->
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
