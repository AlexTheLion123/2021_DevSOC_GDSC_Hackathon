<script>
    export let logo;
    import Stars from '$lib/components/Stars.svelte';
    export let rating;
</script>


<div class="job">
    <div class="picture-content">
        <h3><slot name="companyName"/></h3>
        <img src={logo} alt="logo">
    </div>
    <div class="text-content">
        <div class="description">
            <slot name="description"/>
            <slog name="requiredSkills"/>
        </div>
        <div class="job-foot-content">
            <span><b># Applicants </b><slot name="numApplicants"/></span>
            <span><b>Reviews </b><slot name="reviews"/></span>
            <Stars {rating}/>
        </div>
    </div>
</div>

<style>
    .job {
		width: 100%;
        max-width: 900px;
		border: 1px solid #aaa;
		border-radius: 2px;
		box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
		padding: 1em;
		margin: 0 0 1em 0;

        display: grid;
        grid-template: 1fr / 1fr 3fr;

        transition: 1s all ease;
	}

    .job:hover {
        transform: scale(1.05);
    }

    img {
        height: 4rem;
    }
    

    .picture-content, .text-content {
        padding: 5px; 
        flex: 1 1 150px;

    }
    .text-content {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        flex: 1 1 500px;
    }
    
    .job-foot-content {
        display: flex;
        justify-content: flex-end;
    }

    .job-foot-content > span {
        margin: 0 20px;
    }

    h3 {
        margin: 0;
        font-size: 1rem;
    }
    h4 {
        margin: 0;
        color: rgb(133, 125, 125);
        font-size: 0.8rem
    }
</style>