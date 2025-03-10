<!DOCTYPE html>
<html lang="kk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Shera TV 🧌</title>
<style>
body {
    font-family: Arial, sans-serif;
    background: url('https://www.connectedone.net/wp-content/uploads/2023/04/16-hafta.jpg') no-repeat center center fixed;
    background-size: cover;
    text-align: center;
    color: white;}
.container {
    max-width: 1000px;
    margin: auto;
    padding: 20px;
    background: rgba(0, 0, 0, 0.7);
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
    border-radius: 10px;}
.header {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 10px;}
.search-box {
    padding: 8px;
    border-radius: 5px;
    border: none;
    width: 200px;
    margin-bottom: 10px;}
.genre-filter {margin-bottom: 20px;}
.genre-filter button {
    padding: 5px 10px;
    margin: 5px;
    border: none;
    border-radius: 5px;
    cursor: pointer;}
.item { margin: 20px 0; }
img {
    max-width: 100%;
    border-radius: 10px;
    transition: transform 0.3s;}
img:hover { transform: scale(1.05); }
.movies {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;}
.movie { width: 30%; display: block; }
</style>
<script>
function searchMovies() {
let input = document.getElementById('search').value.toLowerCase();
let movies = document.getElementsByClassName('movie');
    for (let i = 0; i < movies.length; i++) {
        let title = movies[i].getElementsByTagName('h2')[0].innerText.toLowerCase();
        if (title.includes(input)) {
            movies[i].style.display = "block";
        } else {
            movies[i].style.display = "none";
        }
    }
}
function filterGenre(genre) {
let movies = document.getElementsByClassName('movie');
for (let i = 0; i < movies.length; i++) {
if (movies[i].classList.contains(genre) || genre === 'all') {
movies[i].style.display = "block";} 
else {
movies[i].style.display = "none";}}}
</script>
</head>
<body>
<div class="container">
<div class="header">
<h1>SHERA TV</h1>
<input type="text" id="search" class="search-box" onkeyup="searchMovies()" placeholder="Фильм іздеу...">
<div class="genre-filter">
    <button onclick="filterGenre('all')">Барлығы</button>
    <button onclick="filterGenre('action')">Боевик</button>
    <button onclick="filterGenre('horror')">Қорқынышты</button>
    <button onclick="filterGenre('fantasy')">Фантастика</button>
    <button onclick="filterGenre('comedy')">Комедия</button>
</div>
</div>
<div class="movies">
    <div class="movie action"><h2>Джон Уик</h2><a href="https://yandex.kz/video/preview/9358055194736213810"><img src="https://upload.wikimedia.org/wikipedia/en/9/98/John_Wick_TeaserPoster.jpg" alt="Джон Уик"></a></div>
    <div class="movie horror"><h2>Спуск 2</h2><a href="https://yandex.kz/video/preview/8160407009032786941"><img src="https://b1.filmpro.ru/c/64568.jpg" alt="Спуск 2"></a></div>
    <div class="movie fantasy"><h2>Гарри Поттер</h2><a href="https://yandex.kz/video/preview/16512356797905321277"><img src="https://cdn1.ozone.ru/s3/multimedia-p/6842439997.jpg" alt="Гарри Поттер"></a></div>
    <div class="movie fantasy"><h2>Мстители: Финал</h2><a href="https://yandex.kz/video/preview/5876035674035250250"><img src="https://upload.wikimedia.org/wikipedia/en/0/0d/Avengers_Endgame_poster.jpg" alt="Мстители"></a></div>
    <div class="movie fantasy"><h2>Интерстеллар</h2><a href="https://yandex.kz/video/preview/18404940530957707945"><img src="https://upload.wikimedia.org/wikipedia/en/b/bc/Interstellar_film_poster.jpg" alt="Интерстеллар"></a></div>
    <div class="movie action"><h2>Тенет</h2><a href="https://yandex.kz/video/preview/12882194791606118358"><img src="https://upload.wikimedia.org/wikipedia/en/1/14/Tenet_movie_poster.jpg" alt="Тенет"></a></div>
    <div class="movie horror"><h2>Апокалипсис Z</h2><a href="https://yandex.kz/video/preview/6902494619923121203"><img src="https://scarfilm.org/wp-content/uploads/2024/11/8bl9cxrpf40xnmvdlefxpxm3gmn.jpg" alt="Апокалипсис Z"></a></div>
    <div class="movie action"><h2>Гладиатор</h2><a href="https://yandex.kz/video/preview/3190058511542243492"><img src="https://www.ecranlarge.com/content/uploads/2020/07/5gjou3t2qrznujqjcg7fqdmi76t-349.jpg" alt="Гладиатор"></a></div>
    <div class="movie fantasy"><h2>Аватар</h2><a href="https://yandex.kz/video/preview/8320136653463205208"><img src="https://upload.wikimedia.org/wikipedia/en/d/d6/Avatar_%282009_film%29_poster.jpg" alt="Аватар"></a></div>
    <div class="movie comedy"><h2>Мистер Бин</h2><a href="https://yandex.kz/video/preview/9406151978274509576"><img src="https://avatars.mds.yandex.net/get-kinopoisk-image/1777765/245e6ff9-dd0f-4780-a1ae-6d556d079faa/1920x" alt="Мистер Бин"></a></div>
    <div class="movie horror"><h2>Заклятие</h2><a href="https://yandex.kz/video/preview/10729949107758382156"><img src="https://i2.wp.com/image.tmdb.org/t/p/w1280/uxjkMGY6DOVzL2Bm0L9sNNstc2w.jpg" alt="Заклятие"></a></div>
    <div class="movie action"><h2>Трансформеры</h2><a href="https://yandex.kz/video/preview/14141595724757596778"><img src="https://upload.wikimedia.org/wikipedia/en/6/66/Transformers07.jpg" alt="Трансформеры"></a></div>
</div>
</div>
</body>
</html>

