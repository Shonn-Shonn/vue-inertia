<template>
        <h3 class="text-4xl font-bold">Users</h3>
   <div style="margin-top:600px">
        <h3>The current time is {{ time }}.</h3>
        <Link href="/users" class="text-blue-500" preserve-scroll>Refresh</Link>
   </div>
</template>

<script>

    import { Link } from '@inertiajs/vue3';

    export default{
        props : {
            time: String
        },
    }
</script>

