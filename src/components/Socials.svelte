<a href={url} class="button"> {icons} </a>

<style>

    a.button {
		background-color: #418FDE;
		border: none;
		color: #fff;
        font-weight: bold;
		padding: 15px 15px;
		line-height: 24px;
		display: inline-flex;
		font-size: 16px;
        width: 18px;
        height: 18px;
		border-radius: 50%;
        text-align: center;
        justify-content: center;
        align-items: center;
        margin-left: 12px;
        margin-right: 12px;
	}

</style>

<script>
    export let icons;
    export let url;
</script>