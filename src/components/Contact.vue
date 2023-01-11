<template>
  <section id="contact">
      <div class="contact-img">
          <div>
              <NavBar/>
              <div class="btn-group p-2" role="group" aria-label="Basic outlined example">
                <a href="#testimonials" type="button" class="btn btn-outline-dark"><i class="fa-solid fa-arrow-up"></i></a>
                <a href="#home" type="button" class="btn btn-outline-dark"><i class="fa-sharp fa-solid fa-house"></i></a>
              </div>
              <h3>Thank you for Reviewing my portfolio</h3>
              <h6>Any feedback will be highly appreciated</h6>
          </div>
          <div class="container">
              <form action="https://formspree.io/f/mbjbywlp" method="post">
                <label for="name">Name</label>
                <input type="text" id="name" name="name" placeholder="Enter your name">
                <label for="Surname">Surname</label>
                <input type="text" id="surname" name="surname" placeholder="Enter your surname">
                <label for="email">Your Email address</label>
                <input type="text" id="email" name="email" placeholder="Enter your email">
                <label for="lname">Your Contact Number </label>
                <input type="text" id="number" name="number" placeholder="Enter your number">
                <label for="topics">Topics you would like to discuss</label>
                <select id="topics" name="topics">
                  <option value="Need help with my Code">Need help with my Code</option>
                  <option value="Future Business affairs">Future Business affairs</option>
                  <option value="Something personal">Something personal</option>
                </select>
                <label for="subject">Subject</label>
                <textarea id="subject" name="subject" placeholder="Write something.." style="height:100px"></textarea>
                <center><input type="submit" value="Submit"></center>
              </form>
            </div>
      </div>
  </section>
</template>
<script>
import NavBar from '@/components/NavBar.vue'
export default {
  name: 'Contact',
  components: {
      NavBar
  }
}
</script>
<style scoped>
#contact {
  height: 140vh;
  width: 100%;
}
* {
  box-sizing: border-box;
}
h2, h3, h6, p {
  text-align: center;
  color: black;
}
.contact-img {
  background-image: linear-gradient(white, rgb(216, 191, 191));
  height: 140vh;
}
label {
  color: black;
}
input[type=text], select, textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}
input[type=submit] {
  background-color: transparent;
  color: black;
  padding: 12px 20px;
  border: 1px solid white;
  border-radius: 4px;
  cursor: pointer;
}
input[type=submit]:hover {
  background-color: white;
  color: black;
}
.container{
  width: 100%;
  padding: 30px 30px 50px;
  background-color: transparent;
  border: 2px solid rgba(255,255,255,0.06);
  border-radius: 10px;
  box-shadow: 0 20px 30px rgba(0,0,0,0.2);
  backdrop-filter: blur(10px);
  height: auto;
}
</style>