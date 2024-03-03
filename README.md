# 21f-9064-wesites-html
portfolio
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HarisFarooq</title>
  <link rel="icon" href="portfolio/Haris-design-amped-name.png" type="image/png">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/css/bootstrap.min.css"
    integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>
  <style>
    body {
      background-color: #f8f9fa;
    }

    .navbar {
      background-color: #343a40;
    }

    .navbar-dark .navbar-brand {
      color: #17a2b8;
      font-size: 24px;
      font-weight: bold;
    }

    .navbar-dark .navbar-nav .nav-link {
      color: #17a2b8;
    }

    .navbar-dark .navbar-toggler-icon {
      background-color: #17a2b8;
    }

    .haris {
      background-image: url('your-background-image.jpg'); /* Add your background image URL here */
      background-size: cover;
      background-position: center;
      height: 200px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: rgb(15, 12, 12);
      text-align: center;
    }

    #heading {
      font-size: 2rem;
      margin-top: 10px;
    }

    .logo {
      max-height: 80px;
      margin-right: 10px;
      height: 50px;
      border-radius: 180px;
    }

    .images h1 {
      text-align: center;
      color: gray;
    }

    .btn-primary:hover {
      background-color: rgb(20, 116, 49);
    }

    /* Updated Footer Styling */
    footer.haris {
      background-color: #343a40; /* Updated color */
      padding: 20px 0;
      color: white;
      text-align: center;
      border-top: 2px solid #17a2b8; /* Border color matching navbar brand color */
    }
  </style>
</head>

<body>
  <nav class="navbar navbar-expand-lg navbar-dark">
    <a class="navbar-brand" href="#">HarisFarooq</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
      aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Projects</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </div>
  </nav>

  <header class="haris">
    <div>
      <img src="portfolio/modern-pc-logo-icon-design-with-blue-vector.jpg" alt="Logo" class="logo">
      <marquee>
        <h2 id="heading">Personal Portfolio</h2>
      </marquee>
    </div>
  </header>

  <div class="container">
    <div class="images">
      <marquee><i>
          <h1> My name is Haris Farooq</h1>
        </i></marquee>
      <img src="portfolio/Creating-Your-Own-Website.avif" class="img-fluid" alt="Responsive Image">
    </div>
  </div>

  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="card mb-3">
          <img class="card-img-top" src="portfolio/what-is-github-1-1.png" alt="Card image">
          <div class="card-body">
            <h4 class="card-title">GitHub</h4>
            <p class="card-text">Check out my GitHub repository.</p>
            <a href="https://github.com/haris461/pf-project-connect-4.git" class="btn btn-primary" target="_blank">Visit
              GitHub</a>
          </div>
        </div>
      </div>

      <div class="col-md-6">
        <div class="card mb-3">
          <img class="card-img-top" src="portfolio/th.jfif" alt="Card image">
          <div class="card-body">
            <h4 class="card-title">Email</h4>
            <p class="card-text">Contact me via email.</p>
            <a href="https://mail.google.com/mail/u/0/#inbox" class="btn btn-primary">Send Email</a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"
    integrity="sha384-cU5YxB4hZzjEtxZ3Z5n3EJoPgBS3fBszCIpPfd/cS8qWGGI6FLaH5CL8Ypx0t5Jg" crossorigin="anonymous"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/js/bootstrap.min.js"
    integrity="sha384-J6eJqIiDqTZh2BdBjtmaUerpj2fn2Jq4qwmC5g8BD2L3U5hRS2Yg4UfKGGOlRkX" crossorigin="anonymous"></script>

  <script>
    $(document).ready(function () {
      $(".btn-primary").click(function () {
        $(".btn-primary").removeClass("clicked");
        $(this).addClass("clicked");
        var cardTitle = $(this).closest('.card').find('.card-title').text();
        var synth = window.speechSynthesis;
        var utterance = new SpeechSynthesisUtterance("Button in the " + cardTitle + " card clicked!");
        synth.speak(utterance);
      });
    });
  </script>

  <!-- Updated Footer -->
  <footer class="haris mt-5">
    <div class="container">
      <p class="text-center text-white">&copy; 2024 Haris Farooq. All Rights Reserved.</p>
      <p class="text-center">Designed with ❤️ by Haris</p>
    </div>
  </footer>
</body>

</html>
