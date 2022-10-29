<script>
    let skills = [
        {
            id: 1,
            name: 'HTML'
        },
        {
            id: 2,
            name: 'CSS'
        },
        {
            id: 3,
            name: 'JavaScript'
        }
    ]
</script>

<style>
    .Skills{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    ul{
        margin: 0;
        padding: 0;
        list-style: none;
    }

</style>

<div class="Skills">
    <ul>
        {#each skills as {name}, i}
            <li>{name}</li>
        {/each}
    </ul>
</div>