<template>
  <div class="portfolio_tile">
    <div class = "inside_box">
      <img
        class="tile_image"
        :src="require('@/assets/' + image + '')"
        alt="Portfolio"
      />
    </div>
    <div class = 'tile_text_container'>
        <p class = 'port_head_text'>{{ project_title }}</p>
        <p class = 'port_sub_text'>{{ project_desc }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "PortfolioTile",
  props: {
    image: String,
    project_title : String,
    project_desc : String,
  },
};
</script>

<style>
.portfolio_tile {
  background-color: #ffffff;
  box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);
  border-radius: 2%;
  height: auto;
  padding: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.inside_box{
    background-color: #f8f8f8;
    display: flex;
    height: max-content;
    padding: 10px;
    justify-content: center;
    align-items: center;
    height: 90%;
    width: 90%;
    border-radius: 5px;
}

.tile_image {
    display: flex;
  width: 95%;
  height: 90%;
  border-radius: 5px;
  box-shadow: 1px 1px 1px 1px rgba(0, 0, 0, 0.2);
}

.tile_text_container{
    padding: 10px 0 0 10px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 95%;
}

.tile_text_container p{
    margin: 0;
    padding: 5px 0;
}

.port_head_text{
    color: #263228;
    font-weight: 500;
    font-size: 14pt;
    text-align: left;
}

.port_sub_text{
    color: #9ba4b5;
    font-weight: 500;
    font-size: 14pt;
    text-align: left;
}
</style>