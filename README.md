 var x= document.getElementById("location");
            var p1=2;
            var p2=3;
            var p3=4;  
    function getlocation() {  
        if(navigator.geolocation){  
            navigator.geolocation.getCurrentPosition(showPosition)  
          }  
        else  
        {  
             alert("Sorry! your browser is not supporting")  
         } }  
       
     function showPosition(position){  
       var x = "Your current location is (" + "Latitude: " + position.coords.latitude + ", " + "Longitude: " +    position.coords.longitude + ")";  
                document.getElementById("location").innerHTML = x; 
               let age= prompt("please enter your age ");
               if(age<=50){
                 
                if(position.coords.latitude<=17.6868159 && p1<=3)
                {
                  alert("Recommended platform is 1")
                }
                else if(position.coords.latitude<=18.6868159 && p2<=4)
                {
                    alert("Recommended platform is 2")
                }
                else if(position.coords.latitude<=19.5849012 && p3<=2)
                {
                    alert("Recommended platform is 3")
                }
                else
                {
                    alert("Recommended platform is 4")
                }
            }
            else
            {
                if(position.coords.latitude<=17.6868159 )
                {
                  alert("Recommended platform is 1")
                }
                else if(position.coords.latitude<=18.6868159 )
                {
                    alert("Recommended platform is 2")
                }
                else if(position.coords.latitude<=19.5849012 )
                {
                    alert("Recommended platform is 3")
                }
                else
                {
                    alert("Recommended platform is 4")
                }
                
            }

               
     }      </script>
