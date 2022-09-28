<template>
  <section>
    <a name="Gallery"></a>
    <div></div>
    <div>
      <h1>Installations and flooring projects by IDYLLIC</h1>
    </div>

    <div>
      <ul class="image-gallery">
        <li>
          <img src="../assets/images/img1.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img2.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img3.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img4.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img9.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img12.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img13.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img14.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img16.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img19.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img20.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img22.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img23.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img24.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img26.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img27.jpeg" />
        </li>
        <li>
          <img src="../assets/images/img28.jpeg" />
        </li>
        <li>
          <img src="../assets/images/image1.jpg" />
        </li>
        <li>
          <img src="../assets/images/image2.jpg" />
        </li>
        <li>
          <img src="../assets/images/image3.jpg" />
        </li>
        <li>
          <img src="../assets/images/image4.jpg" />
        </li>
        <li>
          <img src="../assets/images/image5.jpg" />
        </li>
        <li>
          <img src="../assets/images/image6.jpg" />
        </li>
        <li>
          <img src="../assets/images/image7.jpg" />
        </li>
      </ul>
    </div>
  </section>
</template>



<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
}
h1 {
  font-size: 30px;
  font-weight: 600;
  font-family: Josefin Sans;
  margin-bottom: 50px;
  text-align: center;
}

.heading-text {
  margin-bottom: 2rem;
  font-size: 2rem;
  text-align: center;
}

.heading-text span {
  font-weight: 100;
}

ul {
  list-style: none;
}

/* Responsive image gallery rules begin*/

.image-gallery {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 10px;
  widows: 100%;
  padding-bottom: 40px;
}

.image-gallery > li {
  flex-basis: 350px; /*width: 350px;*/
  position: relative;
  cursor: pointer;
}

.image-gallery::after {
  content: "";
  flex-basis: 350px;
}

.image-gallery li img {
  object-fit: cover;
  width: 100%;
  height: 300px;
  vertical-align: middle;
  border-radius: 5px;
}
</style>