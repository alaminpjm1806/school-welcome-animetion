<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Slider</title>
<style>
    .container {
        text-align: center;
    }
    .slider {
        position: relative;
        max-width: 1200px;
        margin: 0 auto;
        overflow: hidden;
    }
    .slider img {
        width: 100%;
        height: auto;
        display: none;
    }
    .slider img:first-child {
        display: block;
    }
</style>
</head>
<body>

<div class="container">
    <section id="home">
        <h2>Welcome/স্বাগত </h2>
        <div class="slider">
            <img src="https://via.placeholder.com/1200x400/0d47a1/ffffff?text=Welcome+to+Our+School" alt="Welcome to Our School">
            <img src="https://via.placeholder.com/1200x400/1976d2/ffffff?text=High+Quality+Education" alt="High Quality Education">
            <img src="https://via.placeholder.com/1200x400/0d47a1/ffffff?text=Join+Us+Today" alt="Join Us Today">
        </div>
    </section>
</div>

<script>
    // JavaScript for automatic image sliding
    const images = document.querySelectorAll('.slider img');
    let currentIndex = 0;

    setInterval(() => {
        images[currentIndex].style.display = 'none';
        currentIndex = (currentIndex + 1) % images.length;
        images[currentIndex].style.display = 'block';
    }, 3000); // Change image every  seconds
</script>

</body>
</html> 
