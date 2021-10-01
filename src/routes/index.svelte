<script>
let name = 'world';
import Student from '../components/Student.svelte';
const jobs = ["job1", "job2", "job3"];
</script>

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


