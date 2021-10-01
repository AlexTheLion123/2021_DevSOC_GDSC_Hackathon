<script>
    export let isYellow;
</script>

<svg height="25" width="23" class="star rating" data-rating="1" class:isYellow>
    <polygon points="9.9, 1.1, 3.3, 21.78, 19.8, 8.58, 0, 8.58, 16.5, 21.78" style="fill-rule:nonzero;" class:isBlank={isYellow == false}/>
</svg>

<style type="scss">
    
    .isYellow {
        fill: #ffd055;
    }

    .isBlank {
        fill: #d8d8d8;
    }

</style>