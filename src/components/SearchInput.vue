<template>
  <div class="searchWrapper">
    <Claim />
    <div class="search">
      <input id="search" name="search" v-model="searchValue" @input="handleInput"/>
    </div>
  </div>
</template>

<script>

export default {
  name: 'SearchInput',
};
</script>

<style lang="scss" scoped>
  .searchWrapper {
    margin-top: 50px;
    display: flex;
    flex-direction: column;
    width: 200px;
  }
  input {
    height:30px;
    border: 0;
    background: none;
    border-bottom: 1px solid black;
  }
</style>
