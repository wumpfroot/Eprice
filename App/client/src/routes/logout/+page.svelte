<script>
    let { data, form } = $props();
</script>


<h1 id="minorheading" class="text-center"><!--class="text-xl pb-4"> h2-->
    Confirm your logout
</h1>

{#if form?.error}
    <div class="alert alert-error">
        {form.error}
    </div>
{/if}

{#if form?.message}
    <div class="alert alert-success">
        {form.message}
    </div>
{/if}


<form method="POST" action="?/logout">
    <button class="w-full btn preset-filled-primary-500" type="submit">Logout</button>
</form>

