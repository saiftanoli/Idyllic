<template>
  <div>
    <a name="Home"></a>
    <figure class="relative cursor-pointer w-full bg-black">
      <img
        class="w-full bg-black"
        src="../assets/images/hardwood-flooring-london.jpg"
      />
      <figcaption class="figure">
        <p>
          Sustainably-sourced,<br />
          handcrafted, Cornish<br />
          engineered flooring
        </p>
      </figcaption>
    </figure>

    <div class="transform-div">
      <img
        class="img"
        src="../assets/images/engineered-flooring-cornwall-2.jpg"
      />
      <div style="width: 650px">
        <h1 class="t-heading">Transform your home</h1>
        <p class="mt-6 t-para">
          Idyllic offers exclusive Tregothan Oak, Olive Ash, reclaimed Douglas
          Fir and Pitch Pine flooring with unparalleled stability, finish and
          durability to present stunning floors of genuine, lasting quality.
        </p>

        <a
          href="#Gallery"
          class="
            inline-flex
            justify-center
            items-center
            p-5
            font-medium
            text-gray-900
            hover:text-indigo-600
          "
        >
          <span class="w-full">Watch Idyllic projects</span>
          <svg
            aria-hidden="true"
            class="ml-3 w-6 h-6"
            fill="currentColor"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              fill-rule="evenodd"
              d="M12.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-2.293-2.293a1 1 0 010-1.414z"
              clip-rule="evenodd"
            ></path>
          </svg>
        </a>
      </div>
    </div>
    <div class="tiles">
      <a class="tile"
        ><img class="image" src="../assets/images/IMG-20160924-WA0008-1.jpg" />
        <div class="details">
          <span class="font-sans heading">Tregothnan Oak</span
          ><span class="font-mono"
            >Exclusive oak flooring from Lord Falmouth's Tregothnan Estate</span
          >
        </div></a
      ><a class="tile"
        ><img class="image" src="../assets/images/douglas-fir-cornwall.jpg" />
        <div class="details">
          <span class="font-sans heading"> Douglas Fir</span
          ><span class="font-mono"
            >120-year old reclaimed Douglas Fir durable and full of
            character</span
          >
        </div></a
      ><a class="tile"
        ><img class="image" src="../assets/images/IMG_1018-scaled.jpg" />
        <div class="details">
          <span class="font-sans heading">Olive Ash</span
          ><span class="font-mono"
            >Deeply exotic engineered Olive Ash for a lighter texture and
            feel</span
          >
        </div></a
      ><a class="tile"
        ><img class="image" src="../assets/images/IMG_0149-scaled.jpg" />
        <div class="details">
          <span class="font-sans heading">Parquet flooring</span
          ><span class="font-mono"
            >Elegant engineered handcrafted parquet and chevron flooring</span
          >
        </div></a
      >
    </div>
  </div>
</template>
<style scoped lang="scss">
@import url(//codepen.io/chrisdothtml/pen/ojLzJK.css);
@import url("https://fonts.googleapis.com/css2?family=Josefin+Sans:ital,wght@0,200;0,300;0,400;1,300&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;1,100;1,200;1,300;1,400&display=swap");
@import url('font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;');
@import url('font-family: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";');
$anim-speed: 0.3s;
.transform-div {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 100px;
  align-items: center;
  padding: 50px;
  flex-wrap: wrap;
}
.figure {
  position: absolute;
  font-family: Josefin Sans;
  font-size: 5vw;
  top: 35vw;
  left: 8vw;
  font-weight: 900;
  color: white;
}
.img {
  width: 400px;
  height: 400px;
}
.image {
  height: 350px;
  width: 100%;
}
.heading {
  font-size: 3vw;
  margin-bottom: 15px;
  font-weight: 700;
}
.t-heading {
  margin-top: 20px;
  font-size: 30px;
  font-weight: 500;
  font-family: Josefin Sans;
}
.t-para {
  font-family: Poppins;
  line-height: 2;
  font-size: 18px;
}
.tiles {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 10px;

  .tile {
    display: inline-block;
    margin: 10px;
    height: 350px;
    width: 300px;
    text-align: left;
    opacity: 0.99;
    overflow: hidden;
    position: relative;
    border-radius: 3px;
    box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.05);

    &:before {
      content: "";
      background: linear-gradient(
        to bottom,
        rgba(0, 0, 0, 0) 0%,
        rgba(0, 0, 0, 0.7) 100%
      );
      width: 100%;
      height: 50%;
      opacity: 0;
      position: absolute;
      top: 100%;
      left: 0;
      z-index: 2;
      transition-property: top, opacity;
      transition-duration: $anim-speed;
    }

    img {
      display: block;
      max-width: 100%;
      backface-visibility: hidden;
      -webkit-backface-visibility: hidden;
    }

    .details {
      font-size: 16px;
      padding: 20px;
      color: #fff;
      position: absolute;
      bottom: 0;
      left: 0;
      z-index: 3;

      span {
        display: block;
        opacity: 0;
        position: relative;
        top: 100px;
        transition-property: top, opacity;
        transition-duration: $anim-speed;
        transition-delay: 0s;
      }

      .title {
        line-height: 1;
        font-weight: 600;
        font-size: 18px;
      }

      .info {
        line-height: 1.2;
        margin-top: 5px;
        font-size: 12px;
      }
    }

    &:focus,
    &:hover {
      &:before,
      span {
        opacity: 1;
      }

      &:before {
        top: 50%;
      }

      span {
        top: 0;
      }

      .title {
        transition-delay: 0.15s;
      }

      .info {
        transition-delay: 0.25s;
      }
    }
  }
}
</style>