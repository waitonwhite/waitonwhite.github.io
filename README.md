<head>
  <title>Леопард</title>
</head>
<body>
  <header class="header">Леопард | My little blog</header>
  <div class="content">
    <div>Встроенный контент</div>
    <button class="moreContent">Click for open new content</button>
    <div class="contents">
      <img
        src="https://mymodernmet.com/wp/wp-content/uploads/2019/07/will-burrard-lucas-beetlecam-23-1024x683.jpg"
        style="height: 150px"
      />
      <iframe
        width="420"
        height="315"
        src="https://www.youtube.com/embed/EYVrdomVWKI"
      >
      </iframe>

      <p style="text-align: center">
        Леопард — это большая хищная кошка. Состоит в родстве со львами, тиграми
        и ягуарами. В XX веке был внесён в Красную книгу МСОП, в Красную книгу России, а также в охранные документы других стран. Однако во многих странах Африки относительно высокая численность леопардов позволяет выделять ежегодно квоту на их добычу. 
      </p>
    </div>
  </div>
</body>
<style>
  @import url("https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;500;600;700&display=swap");
  body {
    margin: 0;
    display: flex;
    flex: 1;
    flex-direction: column;
  }
  .header {
    background: yellow;
    padding-left: 10px;
    font-size: 32px;
    font-family: "Dancing Script", cursive;
  }
  .content {
    background: gray;
    margin: 10px;
    padding: 10px;
    min-height: 200px;
    border-radius: 12px;
  }
  .contents {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    display: none;
  }
</style>
<script>
  const button = document.querySelector(".moreContent");
  const content = document.querySelector(".contents");
  button.addEventListener("click", (el) => {
    if (content.style.display == "none") {
      content.style.display = "block";
    } else {
      console.log(content.style.display);
      content.style.display = "none";
    }
  });
</script>
