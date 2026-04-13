<script>
    import MovieCard from "$lib/movieCard.svelte";
    const movies = [
        {
            title: "Spider-Man",
            year: 2002,
            length: "121 Minuten",
            poster: "/images/Spiderman_2002.webp",
        },
        {
            title: "The Dark Knight",
            year: 2008,
            length: "152 Minuten",
            poster: "/images/TheDarkKnight.jpg",
        },
        {
            title: "Spider-Man: No Way Home",
            year: 2021,
            length: "148 Minuten",
            poster: "/images/SpidermanNWH.jpg",
        },
        {
            title: "The Batman",
            year: 2022,
            length: "176 Minuten",
            poster: "/images/TheBatman.jpg",
        },
    ];
</script>

<div class="bg-dark min-vh-100 pt-5 pb-5">
    <div class="container mt-5 text-white">
        <h2 class="mb-4">Unsere Superhelden-Watchlist</h2>

        <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 g-4">
            {#each movies as movie}
                <MovieCard
                    title={movie.title}
                    year={movie.year}
                    length={movie.length}
                    poster={movie.poster}
                />
            {/each}
        </div>
    </div>
</div>
