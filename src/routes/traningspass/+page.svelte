<script>
    import { base } from '$app/paths';
    let traningspass = [{name:"ett pass"}]
</script>

<main>
    {#each traningspass as pass}
        <p>{pass.name}</p>
    {/each}

    <a href="{base}/traningspass/laggtillpass">Lägg Till Pass</a>

</main>

<style>

</style>