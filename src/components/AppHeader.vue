<script>
export default {
  data() {
    return {
      links: [
        {
          name: 'Characters',
          url: '#',
          active: false,
        },
        {
          name: 'Comics',
          url: '#',
          active: false,
        },
        {
          name: 'Movies',
          url: '#',
          active: false,
        },
        {
          name: 'Tv',
          url: '#',
          active: false,
        },
        {
          name: 'Games',
          url: '#',
          active: false,
        },
        {
          name: 'Collectibles',
          url: '#',
          active: false,
        },
        {
          name: 'videos',
          url: '#',
          active: false,
        },
        {
          name: 'fans',
          url: '#',
          active: false,
        },
        {
          name: 'news',
          url: '#',
          active: false,
        },
        {
          name: 'shop',
          url: '#',
          active: false,
        },
      ]
    }
  }
}
</script>
<template lang="">
  <header>
    <div class="container">
      <div class="navbar">
        <div class="logo">
          <a href="">
            <img src="../assets/img/dc-logo.png" alt="">
          </a>
        </div>
        <div class="list">
          <ul>
            <li v-for="(link , index) in links" :key="index">
              <a href="{{link.url}}">{{link.name}}</a>
            </li>
          </ul>
        </div>
      </div>
      
    </div>
  </header>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.navbar {
  display: flex;
  justify-content: space-between;

  .logo {
    a {
      img {
        width: 80px;
        vertical-align: middle;
      }
    }
  }

  .list {
    vertical-align: middle;

    ul {
      list-style-type: none;
      margin: 0;
      display: flex;

      li {
        padding: 0 10px;

        a {
          text-transform: uppercase;
          color: black;
          line-height: 80px;
          font-weight: 600;
          font-size: 12px;

          &:active,
          &:hover {
            color: $primary_color;

          }
        }
      }
    }
  }

}
</style>