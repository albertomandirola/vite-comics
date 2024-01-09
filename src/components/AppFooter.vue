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
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
<footer>
  <div class="top-footer">
    <div class="container">
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
    <div class="container">
      <div class="bottom-footer-inner">
        <div class="my-btn">sign up now!</div>
        <div class="socials">
          <ul>
            <li>Follow us</li>
            <li><i class="fa-brands fa-facebook"></i></li>
            <li><i class="fa-brands fa-twitter"></i></li>
            <li><i class="fa-brands fa-youtube"></i></li>
            <li><i class="fa-brands fa-pinterest"></i></li>
          </ul>
        </div>
      </div>
      

    </div>
    
  </div>
</footer>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.top-footer {
  background-image: url('../assets/img/footer-bg.jpg');
  background-size: cover;


  .top-footer-inner {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-position: right;
    background-repeat: no-repeat;
    display: flex;



    .top-footer-menu {

      padding: 50px 10px;


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

.bottom-footer {
  background-color: darkslategrey;
  font-weight: 600px
}

.bottom-footer-inner {
  @include space-between-vertical-center;
  height: 100px;

  .my-btn {
    border: $primary_color 2px solid;
    padding: 10px;
    text-transform: uppercase;
    color: white;
  }

  ul {
    margin-left: 15px;
    @include orizontal-list;
    color: $primary_color;
    font-size: 20px;

    i {
      padding: 0 10px;
      color: grey;
    }
  }

}
</style>