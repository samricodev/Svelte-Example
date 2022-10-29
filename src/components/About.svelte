<script>
    let someText = `Frontend de peso!`;
    let count = 0;
    let styles = {darkMode : false}

    function incrementCount(){
        count += 1;
    }

    function toggle(){
        styles.darkMode = !styles.darkMode;
        window.document.body.classList.toggle("darkMode");
    }
</script>

<style>
    p{
        text-align: center;
        font-size: 1.2rem;
        color: rgb(129, 129, 129);
    }
</style>

<div class="About">
    {#if !styles.darkMode}
        <p>{someText}</p>
    {:else}
        <p>
            <span>Hello DarkMode</span>
        </p>
    {/if}
    <button on:click={incrementCount}>
        Click {count} {count == 1 ? "time": "times"}
    </button>
    <button on:click={toggle}>-DarkMode-</button>
</div>