<script>
    var a = "a ";
    var b = "b ";
    var c = "c ";
</script>

<h1>HTML Before</h1>
<div>
    Refresh page to see a flickering bug. If you are fast, then you may even stop refreshing and thus get the intended state.
</div>
<br>

{@html a}
{@html b}
{@html c}

<h1>HTML After</h1>

