<script>
    import Navbar from './Navbar.svelte';
</script>

<style>
h1 {
    font-size: 4.5rem;
    text-align: center; 
}

.banner {
    background-image: url('/assets/banner.jpeg');
    background-size: cover;
    background-position: center;
    position: relative;
    height: 72vh;
    color: #1c1c1c;
}

.banner:before {
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    background-color: rgba(137,141,144,.3);
}

.content {
    position: relative;
    height: 100%;
}

.container {
    height: 100%;
    position: absolute;
    top: 0;
    right: 0;
    left: 0;
    display: flex;
    align-items: center;
}
</style>

<header class="banner">
    <div class="content">
        <Navbar />
        <div class="wrapper container">
            <h1>Multichannel ecommerce designed for furniture manufacturers.</h1>
        </div>
    </div>
</header>