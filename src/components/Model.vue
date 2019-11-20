<template>
  <div class="outerWrapper">
    <div class="innerWrapper">
      <div class="photo">
        <img src="https://images-assets.nasa.gov/image/PIA21384/PIA21384~small.jpg">
      </div>
      <div class="description">
        <h2 class="title">Lorem ipsum</h2>
        <p class="description">
          Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum
          Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum
          Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum
          Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum
        </p>
      </div>
    </div>
    <div class="close" />
  </div>
</template>

<script>
export default {
  name: 'Model',
};
</script>

<style lang="scss" scoped>
  .outerWrapper {
    max-width: 100%;
    height: 100%;
    position: fixed;
    top: 0;
    left: 0;
    background: #F6F6F6;
  }
  .close  {
    position:absolute;
    width: 30px;
    height: 30px;
    padding: 30px;
    right: 0;
    top: 0;
    cursor: pointer;

    &::before,
    &::after {
      position: absolute;
      top: 30px;
      right: 20px;
      content: '';
      width: 10px;
      height: 2px;
      background: black;
      display: block;
    }
    &::before {
      transform: rotate(45deg);
    }

    &::after {
      transform: rotate(-45deg);
    }

  }
  .innerWrapper {
    display: flex;
    height: 100%;
    padding: 50px;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
  .photo {
    width: 100%;
    height: auto;
    background: black;
    img {
      width: 100%;
    }
  }
  .description {
    color: #333;
  }


</style>
