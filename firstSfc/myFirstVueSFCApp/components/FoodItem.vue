<template>
    <div v-on:click="countClicks">
        <h2>{{ name }}</h2>
        <p>{{ message }}</p>
        {{ foodName }} <br />
        {{ foodDescription }}

        <img src="../../../apple.png" v-show="isFavorite"/>
        <p > Clicked Counts {{ count }}</p>
    </div>
</template>

<script>
export default {
    data(){
        return {
            name : 'Apples' , 
            message : 'I Like Apples' , 
            count : 0
        }
    } , 
    props : [
        'foodName' ,
        'foodDescription',
        'isFavorite'
    ],
    methods : {
        countClicks(){
            this.count++;
        }
    }
};
</script>

<style>
#app > div {
    border: dashed black 1px;
    display: inline-block;
    margin: 10px;
    padding: 10px;
    background-color: lightgreen;
  }
</style>