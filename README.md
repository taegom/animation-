# animation-
animation 이용해서 실습한 내용
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

