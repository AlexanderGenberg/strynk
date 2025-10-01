<script>
    let valjpass = true
    let gympass = true
    let konditionspass = true

    function vilketpass(pass) {
        valjpass = false
        if (pass == "gympass") {
            gympass = false
        }
        if (pass == "konditionspass") {
            konditionspass = false
        }
    }


</script>

<div class:hide={!valjpass}>
    <button onclick="{vilketpass("gympass")}">Gym Pass</button>
    <p>eller</p>
    <button onclick="{vilketpass("konditionspass")}">Konditions Pass</button>
</div>


<gympass class:hide={gympass}>
    <p>hej</p>

</gympass>

<konditionspass class:hide={konditionspass}>
    <p>hejhej</p>

</konditionspass>

<style>
    .hide {
        display: none;
    }
</style>