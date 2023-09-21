<template>
  <div class="portfolio-container">
    <div class="portfolio-text-container">
      <p class="portfolio-head-text head-text">Portfolio</p>
    </div>
    <div class="portfolio-grid">
      <div class="portfolio-grid-container">
        <PortfolioTile class="one" image="port-temp.jpeg" :project_title="'My E-Commerce Website'" :project_desc="'Full Stack'" />
        <PortfolioTile class="two" image="blog-temp.png" :project_title="'Blog Website Development'" :project_desc="'Front End'" />
        <PortfolioTile class="three" image="admin-temp.png" :project_title="'Admin Dashboard Design'" :project_desc="'Web Design'" />
      </div>
    </div>
  </div>
</template>

<script>

import PortfolioTile from './PortfolioTile.vue';

export default {
  name: "PortfolioSection",
  components : {
    PortfolioTile,
  }
};
</script>

<style>

</style>

