<script context="module">

    var content = [];

    export async function load({ fetch })
    {
        content = ["a ", "b ", "c "];

        return {};
    }
</script>

<h1>HTML Before</h1>

{#each content as c, i}
    {c}
{/each}

<h1>HTML After (behaves strangely)</h1>

