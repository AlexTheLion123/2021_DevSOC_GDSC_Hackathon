<script>
    export let avatar;
</script>


<div class="student">
    <div class="picture-content">
        <h3><slot name="name"/></h3>
        <h4><slot name="catchPhrase"/></h4>
        <img src={avatar} alt="Avatar">
    </div>
    <div class="text-content">
        <div class="description">
            <slot name="description"/>
        </div>
        <div class="student-foot-content">
            <b>Skills</b><slot name="skills"/>
            <b>Reviews</b><slot name="reviews"/>
        </div>
    </div>
</div>

<style>
    .student {
		width: 300px;
		border: 1px solid #aaa;
		border-radius: 2px;
		box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
		padding: 1em;
		margin: 0 0 1em 0;

        display: grid;
        
	}

    

</style>