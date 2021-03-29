<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div class="container wrapInfo">
      <div class="left-div">
          <!-- <img :src="require(`../assets/${imgURL}`)" /> -->
          <!-- <img src="./assets/logo.png"> -->
          <img alt="Bishakha" src="https://avatars.githubusercontent.com/u/48410779?v=4">
      </div>
      <div class="right-div description">
        <h2>
          Hi, I am Bishakha. <br>
          <strong>
            I am currently a senior with a major in Computer Science and minor in Neuroscience aspiring to become a Software Engineer. 
          </strong>
          </h2>
          <span>
          <!-- <button type="button" class="btn btn-outline-success">Resume</button> -->
          <a href="https://ubishakha.github.io/ubishakha-me/Upadhyaya_Resume_2021.pdf" class="btn btn-outline-success" role="button">Resume</a>
          <a href="https://www.linkedin.com/in/bishakha-upadhyaya/" class="btn btn-outline-info" role="button">Linkedin</a>
          <!-- <button type="button" class="btn btn-outline-info">LinkedIn</button> -->
          </span>
      </div>
    </div>
  </div>
  
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    Url: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.left-div {
    float: left;
    /* margin-right: 8px; */
    /* background-color: linen; */
}
.right-div {
    color: #737373;
    max-width: 400px;
}
</style>
