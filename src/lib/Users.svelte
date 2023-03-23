<script>
    const users = [
        {
            id: 1,
            name: "John Wick",
            img: 'https://cdn-icons-png.flaticon.com/512/3135/3135715.png',
            email: 'john@wick.com'
        },
        {
            id: 2,
            name: "Ronald Wick",
            img: 'https://cdn-icons-png.flaticon.com/512/2202/2202112.png',
            email: 'ronald@wick.com'
        },
        {
            id: 3,
            name: "Oliver Wick",
            img: 'https://cdn-icons-png.flaticon.com/512/4140/4140048.png',
            email: 'oliver@wick.com'
        },
        {
            id: 4,
            name: "James Wick",
            img: 'https://cdn-icons-png.flaticon.com/512/4333/4333609.png',
            email: 'james@wick.com'
        },
        {
            id: 5,
            name: "Samantha Wick",
            img: 'https://cdn-icons-png.flaticon.com/512/4140/4140047.png',
            email: 'sami@wick.com'
        },
        {
            id: 6,
            name: "Jeny Wick",
            img: 'https://cdn-icons-png.flaticon.com/512/4140/4140051.png',
            email: 'jeny@wick.com'
        }
    ]
</script>

<div>
    <h1 class="text-2xl text-center mt-10 mb-10">The Users</h1>
    {#each users as {id, name, img, email }, index(id)}
        <div class="flex items-center">
            <img src={img} alt={name} class="m-2">
            <p class="w-full">{name}</p>
            <p>{email}</p>
        </div>        
    {:else}
        <h3>No users found</h3>
    {/each}
</div>


<style>
    img {
        width: 70px;
    }
</style>