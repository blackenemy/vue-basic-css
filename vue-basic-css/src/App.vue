<script >
  export default{
    name:"App",
    data(){
      return{
          Description:"Improve your front-end skills by building projects",
          pictue:"../src/assets/images/image-qr-code.png"
      }
    }
  }
  const photos = [
    "favicon-32x32",
    "image-qr-code"
  ]

</script>

<template>
  <body>
    <div class="card">
      <div class="card-containe">
       <img v-bind:src="pictue">
        <h3>{{ Description }}</h3> 
        <p>Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
      </div>
    </div>
  </body>
    
 

 
</template>

<style scoped>
.card{
    width:19.2rem;
    height:30rem;
    border-radius:1rem;
    display:flex;
    justify-content:center;
    align-items:center;
    background-color:hsl(0, 0%, 100%);
}

.card-container{
   height:93%;
   width:89%;
}
body{
  height:100vh;
  background-color:hsl(212, 45%, 89%);
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  row-gap:1rem;
}
img{
  width:100%;
  height:30%;
  border-radius:10px;
}

h3,p{
  text-align:center;
}

h3{
  font-size:1.3rem;
  font-family: "Outfit", sans-serif;
  font-optical-sizing:auto;
  padding: 0.50rem;
}

p{
  font-size:0.98rem;
  font-family: "Outfit", sans-serif;
  font-optical-sizing:auto;
  font-weight:180;
  font-style:normal;
}
</style>
