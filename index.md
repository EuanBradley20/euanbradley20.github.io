<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
* {
  box-sizing: border-box;
}
h1 {text-align: center;}
h2 {text-align: center;}

.column {
  float: left;
  width: 50%;
  padding: 10px;
  height: 500px;
}

.column2 {
  float: left;
  width: 100%;
  padding: 10px;
  height: 640px;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

body {
    font-family: Garamond, serif;
}

.header {
  padding: 10px 16px;
  background: #272838;
  color: #f1f1f1;
}

.content{
  padding: 16px;
}

.sticky{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
}

.sticky + .content {
  padding-top: 102px;
}

<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="msapplication-TileColor" content="#da532c">
<meta name="theme-color" content="#ffffff">

</style>
</head>
<body style="background-color: #A7B0CA;">

<div class="row">
  <div class="header" id="myHeader">
    <h1>The Quizzicle</h1>
  </div>
  <div class="column" style="background-color: #2B2D42;">
    <h2 style="color:wheat">Next Host</h2>
    <p style="color:wheat">The Next Upcoming Quiz is scheduled to be hosted by: Me!</p>
  </div>
  <div class="column" style="background-color:#8D99AE;">
    <h2>QUIZ CANCELLED</h2>
    <p>This weeks quiz was cancelled in a shocking decision from Quiz leadership</p>
  </div>
  <div class="column2" style="background-color:#EDF2F4;">
    <h2>Total Wins</h2>
    <p>NOTE: These totals are a speculation from reading the history of messages in the Quiz Wizz Messenger chat, I cannot say beyond reasonable doubt that these are accurate</p>
    <table border="1" style="width:100%">
      <tr>
        <th style="width:20%"> <b>Position</b> </th>
        <th style="width:80%"> <b>Team Name</b> </th>
        <th style="width:50%"> <b>Win Total</b> </th>
      </tr>
      <tr>
        <td style="width:20%"> 1.</td>
        <td style="width:50%"> Pinders</td>
        <td style="width:30%"> 15</td>
      </tr>
      <tr>
        <td style="width:20%"> 2.</td>
        <td style="width:50%"> Gem, Kev and Fran</td>
        <td style="width:30%"> 8</td>
      </tr>
      <tr>
        <td style="width:20%"> 2.</td>
        <td style="width:50%">  Colmans</td>
        <td style="width:30%"> 6</td>
      </tr>
      <tr>
        <td style="width:20%"> 3.</td>
        <td style="width:50%"> Hepples</td>
        <td style="width:30%"> 6</td>
      </tr>
      <tr>
        <td style="width:20%"> 4.</td>
        <td style="width:50%"> Euan</td>
        <td style="width:30%"> 6</td>
      </tr>
      <tr>
        <td style="width:20%"> 4.</td>
        <td style="width:50%"> Ayron and Ellie</td>
        <td style="width:30%"> 4</td>
      </tr>
      <tr>
        <td style="width:20%"> 5.</td>
        <td style="width:50%"> Bradleys</td>
        <td style="width:30%"> 4</td>
      </tr>
      <tr>
        <td style="width:20%"> 6.</td>
        <td style="width:50%"> Neve and Cameron</td>
        <td style="width:30%"> 3</td>
      </tr>
    </table>
  </div>
</div>

<script>
  window.onscroll = function() {myFunction()};

  var header = document.getElementById("myHeader");
  var sticky = header.offsetTop;

  function myFunction() {
    if (window.pageYOffset > sticky){
      header.classList.add("sticky");
    } else{
      header.classList.remove("sticky");
    }
  }
</script>

</body>
</html>
