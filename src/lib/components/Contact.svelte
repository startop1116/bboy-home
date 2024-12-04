<script>
  import Footer from "./Footer.svelte";
  import Header from "./Header.svelte";


</script>

<Header/>

<main class="container">
  <h2>최고의 무대를 선사하겠습니다.</h2>
  <div class="contact">
    <figure class="map">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d6310.958276677898!2d127.03476769755756!3d37.73190213798462!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x357cc0b34b41b6a9%3A0xb137586da7271727!2z6rK96riw64-EIOydmOygleu2gOyLnCDrspTqs6jroZw!5e0!3m2!1sko!2skr!4v1733323049687!5m2!1sko!2skr" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
    </figure>
    <address>
      <p>경기도 의정부시 범골로 123번길 11, 3층</p>
      <p>빅브라더스 스튜디오</p>
      <p>Email: <a href="mailto:startop1116@gmail.com">startop1116@gmail.com</a> </p>
      <p>Tel:
        <a href="031-000-0000">031-000-0000</a> /
        <a href="010-000-0000">010-000-0000</a>
      </p>
      <p>Fax: 031-000-0000</p>
    </address>
  </div>
</main>

<Footer/>

<style lang="scss">
  .contact{
    display: flex;
    gap: 75px;
    figure, address{width: 50%;}
    address{
      font-style: normal;
    }
    a{color: inherit;}
  }

  .container{
    background: #fff;
  }

</style>