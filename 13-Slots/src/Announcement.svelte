<script>
    let show = true;

    const hideAlert = () => {
        show = false;
    }
</script>

{#if show}
    <div class="alert">
        50% off all fruit. Sign up for more fruit!
        <button on:click={hideAlert}>Hide</button>
    </div>
{/if}

<style>
	.alert {
        display: flex;
        align-items: center;
        padding: 2px 12px;
        margin: 12px 0;
        border: 2px solid darkslategrey;
        border-radius: 10px;
        font-size: 18px;
        background-color: darkseagreen;
        color: darkslategray;
    }
</style>