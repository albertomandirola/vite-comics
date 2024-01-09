<script>
export default {
  data() {
    return {
      links: [
        {
          name: 'Characters',
          url: '#'
        },
        {
          name: 'Comics',
          url: '#'
        },
        {
          name: 'Movies',
          url: '#'
        },
        {
          name: 'Tv',
          url: '#'
        },
        {
          name: 'Games',
          url: '#'
        },
        {
          name: 'Collectibles',
          url: '#'
        },
        {
          name: 'videos',
          url: '#'
        },
        {
          name: 'fans',
          url: '#'
        },
        {
          name: 'news',
          url: '#'
        },
        {
          name: 'shop',
          url: '#'
        },
      ]
    }
  }
}
</script>
<template lang="">
<footer>
  <div class="top-footer">
    <div class="contaier">
      <div class="top-footer-inner">
        <div class="top-footer-menu">
          <h3>dc comics</h3>
          <ul>
            <li v-for="(link , index) in links" ::key="index">
              <a href="{{link.url}}">{{link.name}}</a>
            </li>
          </ul>
        </div>
        <div class="top-footer-menu">
          <h3>dc comics</h3>
          <ul>
            <li v-for="(link , index) in links" ::key="index">
              <a href="{{link.url}}">{{link.name}}</a>
            </li>
          </ul>
        </div>
        <div class="top-footer-menu">
          <h3>dc comics</h3>
          <ul>
            <li v-for="(link , index) in links" ::key="index">
              <a href="{{link.url}}">{{link.name}}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
  <div class="bottom-footer">
    <button>Sign up</button>
  </div>
</footer>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;

.top-footer {
  background-image: url('../assets/img/footer-bg.jpg');
  background-size: cover;


  .top-footer-inner {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-position: right;
    background-repeat: no-repeat;
    display: flex;



    .top-footer-menu {

      padding: 50px 0;


      h3 {
        color: white;
        text-transform: uppercase;
      }

      ul {
        list-style-type: none;
        margin: 0;

        li {
          padding: 0 5px;

          a {
            color: lightgrey;
            font-size: 10px;
          }


        }
      }
    }

  }
}
</style>