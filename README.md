# SGAO.2
<!DOCTYPE html>
<head>
<script src="/picture/jquery.js"></script>
<link href='https://fonts.googleapis.com/css?family=Londrina+Shadow' rel='stylesheet' type='text/css'>
<style>
body {
  font-family: helvetica, sans-serif;
  margin: 0 auto;
  max-width: 600px;
  background: #232323;
}
div {
  height: 200px;
  background-size: cover;
  position: relative;
  margin: 40px 0 0 0;
  border-radius: 12px;
}
h1 {
  font-family: 'Londrina Shadow', cursive;
  text-align: center;
  font-size: 75px;
  color: #aaaaaa;
  margin: 60px 0 0 0;
}
h2 {
  text-align: center;
  color: #bbbbbb;
  margin: 0px 0 70px 0;
}
p {
  color: rgba(255,255,255,1);
  background: black;
  background: linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  background: -webkit-linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  background: -moz-linear-gradient(bottom, rgba(0,0,0,1), rgba(0,0,0,.4));
  padding: 10px;
  line-height: 28px;
  text-align: justify;
  position: absolute;
  bottom: 0;
  margin: 0;
  height: 30px;
  transition: height .5s;
  -webkit-transition: height .5s;
  -moz-transition: height .5s;
}

small {
  opacity: 0;
}

.show-description p {
  height: 150px;
}

.show-description small {
  opacity: 1;
}

.UiUx{
  background-image: url("http://Chinonso.com/picures/UiUxdesigns.jpg");
}
.logodesigns{
  background-image: url("http://Chinonso.com/pictures/Logodesigns.jpg");
}
.content{
  background-image: url(("http://Chinonso.com/pictures/Contentdeveloper.jpg");
}
.price {
  float: right;
}
@media (max-width: 500px) {
  h1 {
    font-size: 50px;
    margin-top: 20px;
    line-height: 40px;
  }
  h2 {
    font-size: 20px;
    margin: 20px 0 30px 0;
  }
  div {
    margin: 20px 12px 0 12px;
  }
  p {
    font-size: 20px;
    line-height: 24px;
  }
  small {
    font-size: 16px;
  }
}

</style>

</head>

<body>
<h1>Chinonso's Crip</h1>
<h2>a Lagos base Ui/Ux Designer</h2>
<div class="Ui/Ux Design">
  <p>User Experience Design Training <span class="price">N10,000</span><br />
  <small>Proper guide from start to finish of UX design. From Product definition (Ideation), to creating personas, Research, Analysis, Design, Implementation and Project Execution. </small></p>
</div>

<div class="Logo Design">
  <p>Logo Design <span class="price">N5,000</span><br />
  <small>We create simple good looking but unique logo for companies, organisations and co-operate bodies.</small></p>
</div>
  
<div class="Content developer">
  <p>Content Development="price">N3,000</span><br />
  <small>We create articles, biographies, Online content and news for bloggers and media houses.</small></p>
</div>

<script>
  $('div').on('click', function() {
      $(this).toggleClass('show-description');
  });
</script>

</body>
