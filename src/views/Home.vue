<template>
  <div class="home">
    <html>
      <head>
      <meta name="=viewport" content="width=device-width, initial-scale=1.0">
    <title>Vue StyleSheet</title>
    <link rel="stylesheet" type="text/css" href="style.css">
      </head>
      <body>
        <section>
          <div class="content">
            <h2>Vue Js stylish stylesheet</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Assumenda placeat officiis iste consequuntur accusamus ipsum omnis. Culpa deserunt iste voluptatem dolore quod ea esse. Culpa consectetur animi asperiores nobis laboriosam!</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Error sint minima nisi totam ut ex fugiat quod, eaque itaque magni hic, dolor aliquam sapiente illum delectus sequi earum, suscipit qui.</p>
          </div>
        </section>
      </body>
    </html>
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {
  }
}
</script>
<style scoped>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family: 'Open Sans', sans-serif;
}
body
{
  min-height:1000px;
}
section{
  position: relative;
  width: 100%;
  height: 100vh;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 50px;
}
section::before{
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  width: 100vh;
  height: 100vh;
  background: #008dff;
  border-radius: 50%;
  transform-origin: bottom;
  transform:translateX(-50%) scale(4)
}
section .content{
  position: relative;
  z-index: 1;
  max-width: 1000px;
  text-align: center;
}
section .content h2{
  font-family: 'Pacifico', cursive;
  font-size: 3em;
  color: aliceblue;
}
section .content p{
    font-family: 'Pacifico', cursive;
  font-size: 1.2em;
  color: #fff;
}

</style>
