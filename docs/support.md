# Support

Got a question that is not answered in the documentation? A feature request? Or maybe you found
an error in the docs or wish to suggest an article? 

Feel free to contact us by leaving a message.

<div class="container">
<style type="text/css" rel="stylesheet">
* {
  box-sizing: border-box;
}
input[class=contact], textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ccc;
  margin-top: 6px;
  margin-bottom: 16px;
  resize: vertical;
}
input[type=submit] {
  background-color: #4CAF50;
  color: white;
  padding: 12px 20px;
  margin-top: 10px;
  border: none;
  cursor: pointer;
}
input[type=submit]:hover {
  background-color: #45a049;
}
.container {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 10px;
}
</style>
  <div style="text-align:center">
    <h2>Contact Us</h2>
  </div>
  <div class="row">
    <div class="col">
      <script src="https://www.google.com/recaptcha/api.js" async defer></script>
      <form accept-charset="UTF-8" action="https://usebasin.com/f/da246548b26a" enctype="multipart/form-data" method="POST">
        <label for="name">Name</label>
        <input class="contact" type="text" id="name" name="name" placeholder="Your name...">
        <label for="company">Company</label>
        <input class="contact" type="text" id="company" name="company" placeholder="Your company...">
        <label for="email">Email</label>
        <input class="contact" type="text" id="email" name="email" placeholder="Your email...">
        <label for="message">Message</label>
        <textarea id="message" name="message" placeholder="Write something..." style="height:250px"></textarea>
        <div class="g-recaptcha" data-sitekey="6Lew3SMUAAAAAJ82QoS7gqOTkRI_dhYrFy1f7Sqy"></div>
        <input type="submit" value="Submit">
      </form>
    </div>
  </div>
</div>
