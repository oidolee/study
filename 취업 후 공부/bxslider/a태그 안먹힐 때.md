# touchEnabled : (navigator.maxTouchPoints > 0),이것을 옵션으로 넣자
   $(document).ready(function(){
      $('.slider').bxSlider({
        touchEnabled : (navigator.maxTouchPoints > 0),
      });
    });
