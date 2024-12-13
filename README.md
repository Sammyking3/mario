<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>MarioClub</title>
    <style>
      body, ul, li, h1, h2, a{
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
}
header{
    background-color: #f63232;
    padding: 20px;
    text-align: center;
    position: fixed;
    width: 100%;
    z-index: 1;
    top: 0;
    left: 0;
}
header h1{
    color: white;
    border: 8px solid white;
    padding: 6px 12px;
    border-radius: 40px;
    display: inline-block;
}
.banner{
    position: relative;
}
.banner img{
    max-width: 100%;
}
.banner .welcome{
    background-color: #feb614;
    color: white;
    padding: 30px;
    position: absolute;
    left: 0;
    top: 30%;
}
.banner h2{
    font-size: 74px;
}
.banner h2 span{
    font-size: 1.3em;
}
nav{
    background-color: #f4f4f4;
    padding: 20px;
    position: sticky;
    top: 105px;
}
nav ul{
    white-space: nowrap;
    max-width: 1200px;
    margin: 0 auto;
}
nav li{
    width: 25%;
    display: inline-block;
    font-size: 24px;
}
nav li a{
    text-decoration: none;
    color: #4b4b4b;
}
nav li a.join{
    color: #f63232;
}
main{
    max-width: 100%;
    width: 1200px;
    margin: 80px auto;
    padding: 0;
    box-sizing: border-box;
}
article h2{
    color: #f63232;
    font-size: 48px;
}
article p{
    line-height: 2em;
    color: #4b4b4b;
}
.images{
    text-align: center;
    margin: 80px 0;
    white-space: nowrap;
}
.images li{
    display: inline-block;
    width: 40%;
    margin: 20px 5%;
}
.images li img{
    max-width: 100%;
}
section.join{
    background-color: #f4f4f4;
    text-align: center;
    padding: 60px 20px;
    color: #4b4b4b;
}
.join h2{
    font-size: 46px;
}
form input{
    margin: 20px 0;
    padding: 10px 20px;
    font-size: 24px;
    border-radius: 28px;
    border: 4px solid white;
}
footer{
    background-color: #f63232;
    color: white;
    padding: 10px;
    text-align: center;
}
/* pseudo classes */
nav li a:hover{
    text-decoration: underline;
}
.images li:hover{
    position: relative;
    top: -4px;
}
form input:focus{
    border: 4px dashed #4b4b4b;
}
form input:valid{
    border: 4px solid green;
}
article p::first-line{
font-weight: bolder;
font-size: 1.2em;
}
section.join p::first-letter{
    font-weight: bolder;
    font-size: 50px;
}
p::selection{
    background-color: red;
    color: white;
}
p::after{
    content: '...'
}

/* media queries */ 

    @media screen and (max-width: 1400px) {

        .banner .welcome h2 {
            font-size: 60px;
        }
        nav li{
            font-size: 18px;
        }

    }
    @media screen and (max-width: 960px) {

        .banner .welcome h2 {
            font-size: 40px;
        }
        

    }
    @media screen and (max-width: 700px) {

        .banner .welcome {
            position: relative;
            text-align: center;
            padding: 10px;
        }
        .banner .welcome br {
            display: none;
        }
        .banner .welcome h2 {
            font-size: 25px;
        }
        .banner .welcome span {
            font-size: 1em;
        }
        .images li {
            width: 100%;
            margin: 20px auto;
            display: block;
        }
    }

    @media screen and (max-width: 560px) {
        nav li{
            font-size: 20px;
            display: block;
            width: 100%;
            margin: 20px 0;
        }
        header{
            position: relative;
        }
        nav{
            top: 0;
        }
    }
    </style>
  </head>

  <body>
    <header>
      <h1>MarioClub</h1>
    </header>
    <section class="banner">
      <img src="./Assets/banner.png" alt="mariobanner" />
      <div class="welcome">
        <h2>Welcome to <br /><span> MarioClub</span></h2>
      </div>
    </section>
    <nav class="main-nav">
      <ul>
        <li><a href="/join.html" class="join">Join the club</a></li>
        <li><a href="/news.html">Latest news</a></li>
        <li><a href="/games.html">New games</a></li>
        <li><a href="/contact.html">Contact</a></li>
      </ul>
    </nav>
    <main>
      <article>
        <h2>It's me, Mario</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel,
          doloremque porro, inventore sit eveniet quos minima debitis ea quasi
          accusantium modi aut voluptas quaerat velit! Deserunt rerum cumque
          esse officia. Lorem, ipsum dolor sit amet consectetur adipisicing
          elit. Voluptatum eos hic quo nihil explicabo voluptate dolores vero
          similique dolore quaerat ut illum distinctio enim, corporis repellat
          modi amet animi deserunt! Lorem ipsum dolor sit amet, consectetur
          adipisicing elit. Provident veritatis dignissimos obcaecati, rerum
          veniam, voluptatum unde assumenda porro, voluptatem aliquam eum earum
          id suscipit saepe nesciunt ratione nostrum doloribus cumque.
        </p>
      </article>
      <ul class="images">
        <li><img src="./Assets/thumb-1.png" alt="mario thumb 1" /></li>
        <li><img src="./Assets/banner.png" alt="mario thumb 2" /></li>
      </ul>
    </main>
    <section class="join">
      <h2>Join Today!</h2>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Earum
        exercitationem voluptatem soluta vitae aperiam dicta ipsa deserunt?
        Commodi unde hic perferendis doloribus illum. Voluptatem alias ullam
        enim ea at. Magni?
      </p>
      <form>
        <input
          type="email"
          name="email"
          placeholder="Type email & hit enter"
          required
        />
      </form>
    </section>
    <footer>
      <p class="copytight">copyright 2024 MarioClub</p>
    </footer>
  </body>
</html>
