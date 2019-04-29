<template>
  <div>
    <h1>Contact Me</h1>
  <p>
    <ul>
      <li class="contact">Email: {{email}}</li>
      <li class="contact">Website: {{web}}</li>
      <li class="contact">github: {{github}}</li>
      <li class="contact">LinkedIn: {{web}}</li>
      <li class="contact">npm: {{npm}}</li>
      <li class="contact">Phone: {{phone}}</li>
    </ul>
  </p>
  </div>
</template>

<script>
export default {
  name: 'Contact',
  data(){
    return {
      email: 'serdarmustafa1@gmail.com',
      web: 'serdarmustafa.com',
      github: 'https://github.com/SerdarMustafa1',
      linkedin: 'https://www.linkedin.com/in/serdar-mustafa/',
      npm: 'https://www.npmjs.com/package/npm-resume-serdar_mustafa',
      phone: '+372 5554 2347'
    }
  }
}
</script>
<style>
.contact {
margin: 20px;
text-align: justify;
align-self: auto;
margin-top: 30px;
}

h1 {
  margin-bottom: 30px;
}
</style>