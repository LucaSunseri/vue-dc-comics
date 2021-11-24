<template>
  <div>

   <ul>
     <li v-for="(link, index) in linkMenu" :key="index">
       <a :class="{active: link.active}" :href="link.url">{{link.name}}</a>
      </li>
   </ul>
   
  </div> 
</template>

<script>
export default {
  name: 'MenuNav',
  data() {
    return {
      linkMenu: [
        {
          url: '#',
          name: 'CHARACTERS',
          active: false,
        },
        {
          url: '#',
          name: 'COMICS',
          active: true,
        },
        {
          url: '#',
          name: 'MOVIES',
          active: false,
        },
        {
          url: '#',
          name: 'TV',
          active: false,
        },
        {
          url: '#',
          name: 'GAMES',
          active: false,
        },
        {
          url: '#',
          name: 'COLLECTIBLES',
          active: false,
        },
        {
          url: '#',
          name: 'VIDEOS',
          active: false,
        },
        {
          url: '#',
          name: 'FANS',
          active: false,
        },
        {
          url: '#',
          name: 'NEWS',
          active: false,
        },
        {
          url: '#',
          name: 'SHOP',
          active: false,
        }
      ]
    }
  }

}
</script>

<style lang="scss" scoped>
@import "../assets/style/vars.scss";

li {
  display: inline-block;
  margin-left: 15px;
  font-weight: bold;
}

a {
  display: inline-block;
  &:hover, &.active {
    color: $primary-color;
    box-shadow: inset 0 -5px 0 $primary-color;
  }
}

</style>