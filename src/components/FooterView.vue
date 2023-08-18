<template>
    <footer>
        <h2>Happy With The Weather?</h2>
      <p>Feel Free To Check Out My</p>
      <div class="links">
        <div class="link-github">
          <p>Github</p>
          <a href="https://github.com/xderfred"
            ><img src="/public/imgs/github-mark.png" alt="github-mark"
          /></a>
        </div>
        <div class="link-homepage">
          <p>Homepage</p>
          <a href="#">
            <section class="icon-homepage">
              <section class="icon-h">H</section>
            </section>
          </a>
        </div>
      </div>
    </footer>
</template>

<script>
    export default {
        name: "FooterView",
        props: {
            msg: String
        }
    }
</script>

<style scoped>

    footer {
        background-color: blueviolet;
        height: 500px;
        width: 100vw;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-evenly;
      }
      
      footer h2 {
        font-size: 4rem;
      }
      
      footer p {
        font-size: 1.3rem;
      }
      
      .links {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        width: 70%;
      }
      
      .link-github {
        text-align: center;
      }
      
      .link-github a img{
        height: 80px;
      }
      
      .link-homepage a {
        text-decoration: none;
      }
      
      .icon-homepage {
        background-color: #24292F;
        height: 80px;
        width: 80px;
        border-radius: 50px;
        text-align: center;
      }
      
      .icon-h {
        font-size: 50px;
        color: white;
        position: relative;
        top: 50%;
        transform: translateY(-50%);
      }
</style>