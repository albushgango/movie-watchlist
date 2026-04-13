<script>
   
    let { title, year, length, poster } = $props();
</script>

<div class="col">
    <div class="card h-100 text-bg-dark border-secondary">
        <img src={poster} class="card-img-top custom-poster" alt={title}>
        <div class="card-body">
            <h5 class="card-title">{title}</h5>
            <p class="card-text mb-1 text-light">Jahr: {year}</p>
            <p class="card-text text-light">Dauer: {length}</p>
        </div>
    </div>
</div>

<style>
    .custom-poster {
        height: 400px; 
        object-fit: cover;
    }
</style>