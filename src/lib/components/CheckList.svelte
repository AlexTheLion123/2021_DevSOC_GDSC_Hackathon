<script></script>

<div class="container">
    <div class="header">
        <h2>
            Lets put some more content over herewefkalsjfaslkfj asf
        </h2>
    
        <div class="grid-content">
                <i class="fas fa-check-circle"></i>
                <p>sadfl; iksfjasd;lk jfs;lkfj sldkfjsd;aklfj sa;lkfjs ;aklfjas</p>
                
                <i class="fas fa-check-circle"></i>
                <p>sadfl; iksfjasd;lk jfs;lkfj sldkfjsd;aklfj sa;lkfjs ;aklfjas</p>
                
                <i class="fas fa-check-circle"></i>
                <p>sadfl; iksfjasd;lk jfs;lkfj sldkfjsd;aklfj sa;lkfjs ;aklfjas</p>
                
                <i class="fas fa-check-circle"></i>
                <p>sadfl; iksfjasd;lk jfs;lkfj sldkfjsd;aklfj sa;lkfjs ;aklfjas</p>
        </div>

        <div class="register-button">Register</div>
        
    </div>
</div>

<style>
    .container {
        max-width: 1500px;
        margin: auto;
    }

    .header {
        color: white;
        width: 100%;
        text-align: center;
        padding: 80px;
    }

    .grid-content {
        margin: 50px;
        font-size: 3rem;
        color: rgb(109, 238, 109);

        display: grid;
        grid-template:
            1fr
            1fr
            / 1fr 5fr 1fr 5fr;
        grid-gap: 50px;
    }

    p {
        color: white;
        font-size: 1.2rem;
        align-self: start;
        margin: 0;
    }


    .register-button {
      width: 200px;
      height: 50px;
      text-align: center;
      margin: 80px auto;

      background: rgb(144, 144, 248);
      border-radius: 5px;
      color: white;
      font-size: 1.5rem;

      display: grid;
      place-items: center;
  }
</style>