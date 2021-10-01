<script>
let name = 'world';
import Student from '../components/Student.svelte';
const jobs = ["job1", "job2", "job3"];
</script>

<nav>
Our logo
<div class="links">
<a href="#">Home</a>
<a href="#">Jobs</a>
<a href="#">Students</a>
<a href = "#">Login</a>
</div>

</nav>

{#each jobs as job}
<Student >
    <div slot = "name">
    Home
    </div>
    <div slot = "description">
    Cape Town
    </div>
</Student>
{/each}

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
