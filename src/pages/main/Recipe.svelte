<script>
    export let header;
    export let body;
    export let src;
</script>

<div class="body">
    <img src={src} alt="LOL"/>
        <div class="text">
            <div class="title">
                {header}
            </div>
            <div>
                {body}
            </div>
        </div>
</div>

<style>
    .body {
        display: flex;
        flex-direction: column;
        width: 25vw;
        height: 50vh;
        margin-top: 10px;
        background-image: url("https://assets.lightspeedhq.com/img/2019/07/bd804558-martin-widenka-tkfrspt-jdk-unsplash-min.jpg");
    }

    img {
        max-width: 100%;
        max-height: 100%;
    }

    .title {
		text-transform: uppercase;
		font-size: 1em;
		font-weight: 100;
	}

    .text {
        align-items: center;
        flex-direction: column;
        margin: 10px;
    }

    @media (max-width: 700px) {
        .recipe {
            flex-direction: column;
        }
    }
</style>