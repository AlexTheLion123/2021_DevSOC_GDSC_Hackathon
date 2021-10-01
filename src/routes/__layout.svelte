<nav>
Our logo
<div class="links">

<a sveltekit:prefetch href="/">Home</a>
<a sveltekit:prefetch href="/jobs">Jobs</a>
<a sveltekit:prefetch href="/students">Students</a>
<a sveltekit:prefetch href = "#">Login</a>
</div>

</nav>

<style>
nav {
display: flex;
justify-content: space-between;
padding: 10px 30px;
background: #fafafa;
}
a {
margin: 0 20px;
padding: 7px;
text-decoration: none;
}
a:hover {
background: #d0d4d9;
}
</style>