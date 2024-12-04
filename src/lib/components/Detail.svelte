<script>
  import Footer from "./Footer.svelte";
  import Header from "./Header.svelte";

  // news 데이터 가져오는 함수
  import {getNews} from '../../assets/news'
  // params 가져오기(props로 전달)
  export let params = {};

  let news = getNews(Number(params.id))
  
</script>

<Header/>

<main class="container">
  <div class="main-header">
    <h2>{news.title}</h2>
    <p class="date">{news.date}</p>
    <img src={news.detailImgUrl} alt={news.title}/>
  </div>
  <article>
    <p>{@html news.desc}</p>
  </article>
</main>

<Footer/>

<style lang="scss">
 .main-header{
  h2{margin-bottom: 10px;}
  .date{
    margin-bottom: 20px;
    font-size: 15px;}
    color: #666;
 }

 article{
  margin-top: 50px;
 }
  .container{
    background: #fff;
  }
</style>