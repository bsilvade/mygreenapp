<template>
<form name="contact" method="POST" data-netlify="true">
  <p>
    <label>Your Name: <input type="text" name="name" class="input is-medium" /></label>   
  </p>
  <p>
    <label>Your Email: <input type="email" name="email" class="input is-medium"/></label>
  </p>
  <p>
    <label>Message: <textarea name="message" placeholder="Detailed description of your comment, request, etc" rows="8"></textarea></label>
  </p>
  <p>
    <button type="submit">Send</button>
  </p>
</form>
</template>
