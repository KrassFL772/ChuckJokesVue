<template>
  <img alt="Chuck Norris" src="./assets/ChuckNorris.jpg">
  <div>
    <h2>Chuck Norris jokes</h2>
    <ul>
      <li v-bind:key="joke.id" v-for="joke in jokes">{{ joke.value }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data(){
    return { 
      jokes: [
    { value: "Chuck Norris can skydive into outer space." },
    { value: "The chief export of Chuck Norris is pain." },
    { value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
    { value: "Time waits for no man. Unless that man is Chuck Norris." },
    { value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
             ]
    }
  }
}

</script>

<style>
ul {
  list-style-type: none;
  padding: 0;
}

li {
  padding: 10px;
  border-bottom: 1px solid #ccc;
}
</style>
