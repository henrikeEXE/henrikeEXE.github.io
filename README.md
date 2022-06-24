# henrikeEXE.github.io

var model= document.getElementById('formulario');
var btn =  document.getElementsByClassName('add_table')[0];
var close = document.getElementsByClassName("close")[0];
var input =  document.getElementsByTagName("input");
var option = document.getElementsByTagName("option");

function clearcontets(){
    model.style.top="-200%";
    model.stlye.backgroud="rga(0,0,0,0.0)";
    model.style.zIdex=-1;
    document.getElementById('title-form').innerHTML="cadastrode novo usuário"
    document.getElementsByName("action")[0].value="create";
    for(x=0;x<Input.length-1;x++){
        input[x].value="";
    }
    for(x=0;x<input.length;x++){
        option[x].selected=false;
    }
}
   btn.onclick=function() {
       model.style.zIndex= 1;
       model.style.top= 0;
       model.style.backgroud= "rgba(0,0,0,0.8)";
       colore();
   }
   close.onclick=function() {
       clearContets();
   }
   window.onclick=function(event) {
       if(event.target==modal){
       clearContets();
       } 
   }
   //extra
    function colore() {
        var square=document.getElementById("title");
        square.style.backgroundColor="#00bfff";
        setTimeout(limparcor,2000);
    }
    function limparcor() {
        var square=document.getElementById("title");
        square.style.backgroundColor="transparent";
        setTimeout(colore,2000);
    }
