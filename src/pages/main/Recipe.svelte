<script>
    import Img from "svelte-img";
    export let header;
    export let body;
    export let src;
</script>

<div>
    <header>
        {header}
    </header>
    <div>
        {body}
    </div>
    <Img src={src}/>
</div>

<style>
    div {
        margin: 10px
    }
    header {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 1em;
		font-weight: 100;
	}
</style>