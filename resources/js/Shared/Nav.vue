<template>
    <nav class="ml-6">
        <ul class="list-none flex space-x-4">
          
            <li>
                <NavLink href="/" :active="$page.component === 'Home'">Home</NavLink>
            </li>
            <li>
               <NavLink href="/users" :active="$page.component === 'Users'">Users</NavLink>
            </li>
            <li>
               <NavLink href="/settings" :active="$page.component === 'Settings'">Settings</NavLink>
            </li>
            <li>
                <Link href="/logout" method="post" :data="{foo: 'bar'}" as="button" class="text-blue-500 hover:underline">Logout</Link>
            </li>
        </ul>
    </nav>
</template>

<script setup>
    import NavLink from '../Shared/NavLink.vue'
</script>
