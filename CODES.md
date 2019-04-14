# modalPopupMistakes
Mistakes on Modal Pop up [html / css / js]

HTML

      <div class="bg-modal">
        <div class="modal-content">
         <div class="close">+</div>
         <img src="gallery\img/LAST1.jpg" alt="" id="fotopopup">

       </div>
      </div>

CSS

    .bg-modal{
      width: 100%;
      height: 100%;
      background-color: rgba(63,191,63,0.64);
      position: absolute;
      top:0;
      justify-content: center;
      align-items: center;
      display: none;
    }

    .modal-content {
      height: 300px;
      width: 500px;
      background-color: white;
      border-radius: 4px;
      text-align: center;
      padding: 20px;
      position: relative;

    }

    #fotopopup{
     width: 100%;
      }

    .close {
      position: absolute;
      top: 0;
      right: 10px;
      font-size: 42px;
      color: #333;
      transform: rotate(45deg);
      cursor: pointer;
      &:hover {
        color: #666;
      }


JS

    document.getElementById('Avatar15').addEventListener("click", function() {
        document.querySelector('.bg-modal').style.display = "flex";
    });

    document.querySelector('.close').addEventListener("click", function() {
        document.querySelector('.bg-modal').style.display = "none";
    });
