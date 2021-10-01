<nav>
    <div class="nav-wrapper">
        <span>Logo</span>
        <div class="links">
            <a href="/">Home</a>
            <a href="/jobs">Jobs</a>
            <a href="/students">Students</a>
            <span class="login-button">Login</span>
        </div>
        
    </div>
</nav>

<svelte:head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Nunito&display=swap">
    <script src="https://kit.fontawesome.com/30f595e84f.js" crossorigin="anonymous"></script>
</svelte:head>

<slot></slot>

<style>
:global(body) {
    margin: 0;
    /* font: 16px/1.6em -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji"; */
    font-family: 'Nunito';
}

:global(*) {
    box-sizing: border-box;
}

nav {
    display: grid;
    place-items: center;
    background: rgb(241, 241, 241);

    width: 100%;
}

.nav-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 60px;
    background: rgb(241, 241, 241);
    max-width: 1500px;
    width: 100%;
    height: 50px;
}
a {
    margin: 0 20px;
    padding: 7px;
    text-decoration: none;
}
a:hover {
    background: #d0d4d9;
}

.login-button {
    padding: 10px 20px;
    margin-left: 30px;

    background: rgb(144, 144, 248);
    border-radius: 5px;
    color: white;
    font-size: 1.3rem;
    
}

.login-button:hover {
    cursor: pointer;
}
</style>