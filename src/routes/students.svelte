<script context="module">
    export async function load({ fetch }) {
      const res = await fetch('/api');
  
    if (res.ok) return {users: await res.json()};
    return {
      status: res.status,
      error: new Error()
     };
    }
</script>


<script>
    let name = 'world';
    import Student from '../components/Student.svelte';
    const jobs = ["job1", "job2", "job3"];
</script>

<div class="container">
    <div class="container-wrapper">
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
    </div>
</div>

<style>
    .container {
        width: 100%;
        display: grid;
        place-items: center;
    }

    .container-wrapper {
        width: 100%;
        max-width: 1500px;
        padding: 50px 150px;
    }

    
</style>