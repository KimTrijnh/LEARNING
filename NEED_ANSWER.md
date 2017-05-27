1.
https://jsbin.com/soziwisele/edit?html,js,console,output
```
$(document).ready(function(){
    var text=$('input').val();
//why text is not updated 
  $('input').keypress(function(event){
    if(event.which ==13){
      do_type();
    }
  });
  
  function do_type(){
    alert("ok");
    $('#demo').html(text);
  }
  
  
});
```
