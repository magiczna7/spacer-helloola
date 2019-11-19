<template>
  <div class="claimWrapper">
    <h1 class="claim">SPACER</h1>
    <p class="subclaim">
      Begin your journey through our amazing galaxy,
      and discover places you never even heard of.
    </p>
    <p class="subclaim">
      Type antyhing space-related to start.
    </p>
  </div>
</template>

<script>
export default {
  name: 'Claim',
};
</script>

<style lang="scss" scoped>
  .claimWrapper {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .claim {
    font-size: 50px;
    margin: 0;
  }
  .subclaim {
    margin: 20px 0 0 0;
    font-size: 13px;
  }
</style>
