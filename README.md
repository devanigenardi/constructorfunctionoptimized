# constructorfunctionoptimized
javascript function


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <script
  src="https://code.jquery.com/jquery-3.2.1.min.js"
  integrity="sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4="
  crossorigin="anonymous"></script>
</head>
<body>
   <div id="test"></div>
   <script>
      function peopleId(name, id){
      this.name = name;
      this.id = id;
      this.display = function(){
         var container = document.createElement('div');
        $(container).addClass('12-col');
        $(container).html("el numero de empleado es =" + this.id + " y su primer nombre es: " + this.name);
        $('#test').append(container);
      }
    }


    var juan = new peopleId("pepe", 111800389);
    juan.display()
    var maria = new peopleId("maria", 111800564);
    maria.display()
    var diana = new peopleId("diana", 111800222);
    diana.display()

</script>
    
</body>
</html>
