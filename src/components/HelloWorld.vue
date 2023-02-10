<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
 
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      animation : [
        {
          aniName : '어둠의 실력자가 되고싶어서!',
          aniImg : 'ani1.png'
        },
        {
          aniName : '터무니없는 스킬로 이세계방랑밥',
          aniImg : 'ani2.png'
        },
        {
          aniName : '해골기사님은 지금 이세계 모험중',
          aniImg : 'ani3.png'
        },
        {
          aniName : '블루록',
          aniImg : 'ani4.png'
        },
      ]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
