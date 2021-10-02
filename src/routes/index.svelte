<script>
  import Icons from "$lib/components/Icons.svelte"
</script>

<div class="container">
  <section class="main-content">
    
    <div class="main-picture">
      <img id="student-image" src="src/lib/images/student.png" alt="Mountains">
    </div>

    <h1 class = "main-heading">Helping students help you</h1>
    <p class = "main-text">
        Many job requirements demand some level of experience from entry level positions,
        yet newly graduate students lack such an experience.<br>
        Many entrepreneurs and startups struggle with raising capital, yet at the beginning
      of their entrepreneurial journey, they are tasked with many roles, where some come with 
      many challenges.
      <br>
      <br>
      With (name_of_solution), it provides entrepreneurs and students in their penultimate and
      final year a place to connect and work with each other.
    </p>

    <div class="register-button">Register</div>
    
  </section>
  
  <section class="icons">
    <Icons/>
  </section>

  <section class="catch-text">
    Lets say something extremely <strong>catchy</strong> and super <strong>cool</strong> sounding over here. mmmmmmmmmmkay
  </section>
  
  <h1>Contact Us</h1>
</div>


    


<style>

  * {
    margin: 0;
  }
  .container {
    margin: auto;
    padding: 50px;
    max-width: 1500px;

  }

  .main-content {
    display: grid;
    grid-template:
      "mainPicture mainHeading" 1fr
      "mainPicture mainText" 5fr
      "mainPicture registerButton" 2fr
      / 1fr 1fr;
  }

  .main-content #student-image {
    width: 95%;
    height: 100%;
  }

  h1 {
    font-size: 2rem;
  }

  .register-button {
      width: 200px;
      height: 50px;
      text-align: center;

      background: rgb(144, 144, 248);
      border-radius: 5px;
      color: white;
      font-size: 1.5rem;

      grid-area: registerButton;
      place-self: center;

      display: grid;
      place-items: center;
  }
  .main-heading {
    grid-area: mainHeading;
    align-self: start;
    margin: 0;
  } 

  .main-text {
    grid-area: mainText;
    align-self: start;
    margin: 10px 0;
    font-size: 1.2rem;
  }

  .main-picture {
    grid-area: mainPicture;
    justify-self: start;
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

  section.icons {
    display: flex;
    justify-content: space-between;
    margin: 80px 0;
  }

  section.catch-text {
    font-size: 1.7rem;

    text-align: center;
    margin: 100px 0;
  }
</style>