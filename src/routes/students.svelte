<script context="module">
    export async function load({ fetch }) {
      const res = await fetch('/api');
  
        if (res.ok) return {props: {students: await res.json()}};
        return { // if failed
            status: res.status,
            error: new Error()
        };
    }
</script>


<script>
    import Student from '../components/Student.svelte';

    export let students;

</script>

<div class="container">
    <div class="container-wrapper">
        {#each students as {firstName, lastName, catchPhrase, avatar, description, skills, reviews}}
            <Student {avatar}>
                <svelte:fragment slot = "name">{firstName}, {lastName}</svelte:fragment>
                <svelte:fragment slot = "catchPhrase">{catchPhrase}</svelte:fragment>
                <svelte:fragment slot = "description">{description}</svelte:fragment>
                <svelte:fragment slot = "skills">{skills}</svelte:fragment>
                <svelte:fragment slot = "reviews">{reviews}</svelte:fragment>
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