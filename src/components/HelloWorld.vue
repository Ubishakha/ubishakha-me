<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div class="container wrapInfo">
      <div class="left-div">
          <img alt="Bishakha" src="https://avatars.githubusercontent.com/u/48410779?v=4">
      </div>
      <div class="right-div description">
        <h3>
          <p class = "desc">Hi, I am Bishakha. </p>
           <p class = "desc"> I am currently a senior with a major in Computer Science and minor in Neuroscience at Knox College aspiring to be a Software Engineer. 
             My experiences include work in Fullstack Development and Data Analytics.
          </p>
          <p class = "desc">
           I am constantly trying to learn new things and get better at thinking programatically.     
          </p>
          </h3>

          <span class = "buttons">
            <button type="button" class="btn btn-primary" @click="goto('div1')">Timeline</button>
          </span>
          <span class = "buttons">
            <a href="https://ubishakha.github.io/ubishakha-me/resume2021.pdf" class="btn btn-success" role="button">Resume</a>
          </span>
          <span class = "buttons">
              <a href="https://www.linkedin.com/in/bishakha-upadhyaya/" class="btn btn-info" role="button">Linkedin</a>
          </span> 
          <!-- <span class = "buttons">
            <button type="button" class="btn btn-secondary" @click="goto('div1')">More About me</button>
          </span> -->
      </div>
    </div>
  </div>

  <div class="container recognitions" ref="div1">
    <div>
      <h3>Career</h3>
      <p style="margin:0">
        <span><strong>2020: &nbsp;</strong>Global Technology Summer Analyst at Bank of America</span>
      </p>
      <p style="margin:0">
        <span><strong>2020: &nbsp;</strong>Started part-time as fullstack developer at csedresearch.org</span>
      </p>
      <p style="margin:0">
        <span><strong>2019: &nbsp;</strong>Fulltime summer research assistant at csedresearch.org</span>
    </p>
    <p style="margin:0">
      <span><strong>2019: &nbsp;</strong>Started part-time as data curator at csedresearch.org</span>
    </p>
  </div>

  <div>
    <h3>Awards</h3>
    <p style="margin:0">
      <span><strong>Dean's List: &nbsp;</strong>Winter 2018, Winter 2019, Winter 2020, Spring 2020, Fall 2020, Winter 2021 </span>
    </p>
    <p style="margin:0">
      <span><strong>Baker-Velde Student Research Fund Award: &nbsp;</strong>2019</span>
    </p>
    <p style="margin:0">
      <span><strong>GHC Scholar: &nbsp;</strong>2020</span>
    </p>
    <p style="margin:0">
      <span><strong>RTC Fellow &nbsp;</strong>2020/2021</span>
    </p>
  </div>
  <div>
    <h3>Publications</h3>
    <p style="margin:0">
      <span><strong><a href="https://dl.acm.org/doi/10.1145/3372782.3406251">Exploring the Enacted Computing Curriculum in K-12 Schools in South Asia: Bangladesh, Nepal, Pakistan, and Sri Lanka </a>&nbsp;</strong><br>Aug 2020 | ICER/ACM</span>
    </p>
    <p style="margin:0">
      <span><strong> <a href="https://dl.acm.org/doi/10.1145/3328778.3366809">A Longitudinal Analysis of K-12 Computing Education Research in the United States: Implications and Recommendations for Change </a>&nbsp;</strong><br>Feb 2020 | SIGCSE/ACM</span>
    </p>
    <p style="margin:0">
      <span><strong><a href="https://dl.acm.org/doi/10.1145/3328778.3372710">Dynamic Data Visualization for CSEdResearch.org using Tableau and MySQL </a>&nbsp;</strong><br>Feb 2020 | SIGCSE/ACM</span>
    </p>
  </div>
</div>
  
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    Url: String
  },
  methods:{
    goto(refName) {
      var element = this.$refs[refName];
      var top = element.offsetTop;
      window.scrollTo(0, top);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 30px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.desc {
  /* overflow-wrap: break-word; */
  font-size: 25px;
  text-align: left;
}

.left-div {
    float: left;
    /* margin-right: 8px; */
    /* background-color: linen; */
}
.right-div {
    color: #737373;
    max-width: 500px;
}
.recognitions {
  height: 1000px;
  padding: 20px;
  font-size: 20px;
}

.buttons{
  padding: 3px;
}
</style>
