<script>
    export let avatar;
    import Stars from '$lib/components/Stars.svelte';
    export let rating;
</script>


<div class="student">
    <div class="picture-content">
        <h3><slot name="name"/></h3>
        <img src={avatar} alt="Avatar">
    </div>
    <div class="text-content">
        <div class="description">
            <slot name="description"/>
            <h4 class="catchPhrase"><slot name="catchPhrase"/></h4>
        </div>
        <div class="student-foot-content">
            <span><b>Skills </b><slot name="skills"/></span>
            <span><b>Reviews </b><slot name="reviews"/></span>
            <Stars {rating}/>
        </div>
    </div>
</div>

<style>
    .student {
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

    .student:hover {
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
    
    .student-foot-content {
        display: flex;
        justify-content: flex-end;
    }

    .student-foot-content > span {
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

    .catchPhrase {
        visibility: hidden;
    }
</style>