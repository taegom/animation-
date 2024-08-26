# animation-
animation 이용해서 실습한 내용
1. licat
<!DOCTYPE html>
<html lang="ko-KR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title></title>
    <style>
      .licat {
        width: 168px;
        height: 200px;
        border: 4px solid deepskyblue;
        background-image: url(./images/licat.png);
        background-repeat: no-repeat;
        background-size: auto 100%;
        background-position: left top;

        animation-name: move-licat;
        animation-duration: 1s;
        animation-timing-function: steps(6);
        animation-iteration-count: infinite;
      }

      @keyframes move-licat {
        100% {
          background-position: right bottom;
        }
      }
    </style>
  </head>
  <body>
    <div class="licat"></div>
  </body>
</html>

![move-licat](https://github.com/user-attachments/assets/efd4b617-62d8-48ae-bc0b-c954b099044a)


2. cat
   <!DOCTYPE html>
<html lang="ko-KR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>animation 실습</title>
    <style>
      .cat {
        width: 313px;
        height: 436px;
        background-size: auto 100%;

        animation-name: move-cat;
        animation-duration: 2s;
        animation-direction: alternate;
        animation-iteration-count: infinite;

        animation-timing-function: ease;
      }

      @keyframes move-cat {
        0% {
          background-image: url(./images/cat/3.png);
          transform: translateX(0);
        }

        25% {
          background-image: url(./images/cat/2.png);
          transform: translateX(100px);
        }

        50% {
          background-image: url(./images/cat/1.png);
          transform: translateX(200px);
        }

        75% {
          background-image: url(./images/cat/2.png);
          transform: translateX(300px);
        }

        100% {
          background-image: url(./images/cat/3.png);
          transform: translateX(400px);
        }
      }
    </style>
  </head>
  <body>
    <div class="cat"></div>
  </body>
</html>

![move-cat](https://github.com/user-attachments/assets/6346356a-dbd4-4dca-bba2-d5687cd75402)

3. cafe
   <!DOCTYPE html>
<html lang="ko-KR">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>cafe건물 올라오는 애니메이션</title>
    <style>
      .cafe {
        width: 116px;
        height: 180px;
        background-image: url(./images/cafe.png);
        background-size: auto;
        background-repeat: no-repeat;
        background-position: left bottom;

        animation-name: move-cafe;
        animation-duration: 6s;
        animation-iteration-count: infinite;
        animation-timing-function: linear;
        animation-timing-function: steps(33);
      }

      @keyframes move-cafe {
        100% {
          background-position: right top;
        }
      }
    </style>
  </head>
  <body>
    <div class="cafe"></div>
  </body>
</html>

