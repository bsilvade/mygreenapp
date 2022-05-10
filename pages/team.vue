<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Our Team"
      subtitle="Socially responsible"
      image="/uploads/mga-team.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
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
          <div class="tile is-ancestor">
           <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
                <p class="subtitle">
                  <b>Paulo Almeida - IT Back-end</b>
                </p>
              </div>
              <div id="right" style="float:right">
                <figure class=" ">
                  <opti-image
                    :src="require('~/assets/uploads/Paulo Almeida.png').src"
                    :srcset="require('~/assets/uploads/Paulo Almeida.png').srcSet"
                    width="125"
                    height="125"
                  />
                </figure>
              </div>
              <div style="text-align:justify">
                CTO Rabbit Care (FinTech) & previously at Central Retail, Top 15 in Thailand Stock Market.
                <br />
                15+ years in software develop., 10+ startups. 
                <br />
                Lived in Portugal, Spain & Thailand
                <br />
                Master  in Computing Science @ FCUP
                <br />
                Head of Engineering at Pomelo Fashion ($1.5M to $300M)
              </div>
            </article>
          </div>
            <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
                <p class="subtitle">
                  <b>Francisco Ferreira - Business Development</b>
                </p>
              </div>
              <div id="right" style="float:right">
                <figure class=" ">
                  <opti-image
                    :src="require('~/assets/uploads/Francisco Ferreira.png').src"
                    :srcset="require('~/assets/uploads/Francisco Ferreira.png').srcSet"
                    width="125"
                    height="125"
                  />
                </figure>
              </div>
              <div style="text-align:justify">
                Master in Environmental Engineering @ FEUP
                <br />
                Based in Portugal
                <br />
              </div>
            </article>
          </div>
          </div>
           <div class="tile is-ancestor">
            <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
                <p class="subtitle">
                  <b>Francisca Falcão - Product Manager</b>
                </p>
              </div>
              <div id="right" style="float:right">
                <figure class=" ">
                  <opti-image
                    :src="require('~/assets/uploads/Francisca Falcao.png').src"
                    :srcset="require('~/assets/uploads/Francisca Falcao.png').srcSet"
                    width="125"
                    height="125"
                  />
                </figure>
              </div>
              <div style="text-align:justify">
                Master in Environmental Engineering @ FEUP
                <br />
                Based in Portugal
              </div>
            </article>
          </div>
            <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
                <p class="subtitle">
                  <b>Sofia Alves - Marketing & Sales</b>
                </p>
              </div>
              <div id="right" style="float:right">
                <figure class=" ">
                  <opti-image
                    :src="require('~/assets/uploads/Sofia Alves.png').src"
                    :srcset="require('~/assets/uploads/Sofia Alves.png').srcSet"
                    width="125"
                    height="125"
                  />
                </figure>
              </div>
              <div style="text-align:justify">
                Degree in Bachelor's Degree Marketing / Marketing Management 
                <br />
                Visual Merchandising course by University of Arts of London
                <br />
                Key Account Manager, Sales and Visual Merchandiser with 10+ years
                <br />
                Lived in Portugal, UK, Qatar, Singapore & Thailand
              </div>
            </article>
          </div>
          </div>
          <div class="tile is-ancestor">
           <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
                <p class="subtitle">
                  <b>Manuel Heitor - Advisor</b>
                </p>
              </div>
              <div id="right" style="float:right">
                <figure class=" ">
                  <opti-image
                    :src="require('~/assets/uploads/Manuel Heitor.png').src"
                    :srcset="require('~/assets/uploads/Manuel Heitor.png').srcSet"
                    width="125"
                    height="125"
                  />
                </figure>
              </div>
              <div style="text-align:justify">
                Former Minister for Science, Technology and Higher Education of Portugal from 2015 until 2022.
                <br />
                Secretary of State for Science, Technology and Higher Education of Portugal from 2005 until 2011 
                <br />
                Graduated with a PhD in Mechanical Engineering from Imperial College London, and did a post-doctoral at the University of California, San Diego.
              </div>
            </article>
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
