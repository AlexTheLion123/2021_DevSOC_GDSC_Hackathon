<body>
    <h1>Our Mission</h1>
    
    <h2>Problem Statement</h2>
    <p>
        Many job requirements demand some level of experience from entry level positions,
        yet newly graduate students lack such an experience.
    </p>
    <p>
        Many entrepreneurs and startups struggle with raising capital, yet at the beginning
        of their entrepreneurial journey, they are tasked with many roles, where some come with 
        many challenges.
    </p>

    <h2>Solution</h2>
    <p>
        With (name_of_solution), it provides entrepreneurs and students in their penultimate and
        final year a place to connect and work with each other.
    </p>

    <h1>Use Cases</h1>
    <div class="row">
        <div class="column">
          <img src="src/lib/images/code_image.png" alt="" style="width:100%">
          <span class="caption">Students gain real life experience</span>
        </div>
        <div class="column">
          <img src="src/lib/images/business_image.png" alt="" style="width:100%">
          <span class="caption">Entrepreneurs work on solutioins with skilfull youth</span>
        </div>
        <div class="column">
          <img src="src/lib/images/employer_image.png" alt="Mountains" style="width:100%">
          <span class="caption">Opportunity to showcase student's experience to potential employers.</span>
        </div>
      </div>
    
      <h1>Contact Us</h1>

</body>

<style>
    input {
        margin-top: 40px;
        width: 300px;
        padding: 10px;
        background: rgb(253, 253, 253);
        border-radius: 5px;
        font-size: 20px;
        margin-right: 10px;
    }
    h1 {
        color: darkblue;
        text-align: center;
    }
    h2 {
        color: lightblue;
        text-align: center;
    }
    body {
        text-align: center;
    }
    div.item {
    vertical-align: top;
    display: inline-block;
    text-align: center;
    width: 120px;
}
img {
    width: 200px;
    height: 50px;
    background-color: grey;
}
.caption {
    text-align: center;
}
/* Three image containers (use 25% for four, and 50% for two, etc) */
.column {
  float: left;
  width: 33.33%;
  padding: 15px;
}

/* Clear floats after image containers */
.row::after {
  content: "";
  clear: both;
  display: table;
}
</style>