<!DOCTYPE html>
<html>
 <head>
  <meta charset="utf-8">
  <title>dialog</title>
  <style>
   body {
    background: url(/example/image/shark.jpg) no-repeat;
    background-size: cover;
   }
   dialog {
    background: rgba(255, 255, 255, 0.7);
    width: 300px; 
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.5);
    border-radius: 5px;
   }
  </style>
 </head> 
 <body> 
  <button id="openDialog">Открыть окно</button>
  <dialog>
   <p>Полинезийцы называют Млечный путь Манго-Роа-И-Ата, 
      что в переводе с маори означает «Длинная акула на рассвете».</p>
   <p><button id="closeDialog">Закрыть окно</button></p>
  </dialog>
  <script>
   var dialog = document.querySelector('dialog');
   document.querySelector('#openDialog').onclick = function() {
    dialog.show(); // Показываем диалоговое окно
   }
   document.querySelector('#closeDialog').onclick = function() {
    dialog.close(); // Прячем диалоговое окно
   }
  </script>
 </body> 
</html>
