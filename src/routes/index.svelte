<script context="module">

    var content = [];

    export async function load({ fetch })
    {
        content = ["a ", "b ", "c "];

        return {};
    }
</script>

<h1>HTML Before</h1>
<div>
    Refresh page to see a flickering bug. If you are fast, then you may even stop refreshing and thus get the intended state.
</div>
<br>
<div>
    <a href="/fix">Fix this by wrapping in div</a>
</div>
<div>
    <a href="/fix-alt">Fix this by removing @html (note that this is not really an equivalent solution)</a>
</div>
<br>

{#each content as c, i}
    {@html c}
{/each}

<h1>HTML After (behaves strangely)</h1>

