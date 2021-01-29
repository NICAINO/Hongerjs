<script>
    export let header;
    export let body;
    export let src;
</script>

<body>
    <div class="recipe">
        <img src={src} alt={"Pog"} width="500" height="500" style="margin: 10px;"/>
        <div class="text">
            <div class="title">
                {header}
            </div>
            <div>
                {body}
            </div>
        </div>
    </div>
</body>

<style>
    body {
        box-sizing: border-box;
        display: flex;
    }

    .recipe {
        margin: 10px;
        display: flex;
        flex-direction: row;
        border-radius: 10px;
        border-width: 2px;
        border-color: #D0585890;
        border-style: solid;
        width: 75vw;
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