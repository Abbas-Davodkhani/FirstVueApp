<script>
  export default {
    data() {
      return {
        message :  'Hello World !'
      }
    }
  }
</script>

<template>
  <h1>{{message}}</h1>


  <h1>Food</h1>
  <food-item food-name="Apples" food-description="Apples' description" 
  v-bind:is-Favorite="true"
  />
  <food-item food-name="Bananas" food-description="Apples' Bananas" 
  v-bind:is-Favorite="false"
  />
  <food-item food-name="Pears" food-description="Apples' Pears" 
  v-bind:is-Favorite="false"
  />


</template>

<style>
#app > div {
  cursor: pointer;
  border: dashed black 1px;
    display: inline-block;
    width: 120px;
    margin: 10px;
    padding: 10px;
    background-color: lightgreen;
}

</style>
