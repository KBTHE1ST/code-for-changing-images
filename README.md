Ryan's Code for Changing Images
<!DOCTYPE html>
 
<html lang="en">
 
    <body>
        <img src="images/1.png" id="image">
        <button onclick="ChangeImage(1)">Up</button>
        <button onclick="ChangeImage(-1)">down</button>
    </body>
 
 
 
</html>
 
<script>
 
    currentIndex = 1
 
    function ChangeImage(by)
    {
        currentIndex += by
 
        if(currentIndex < 1) currentIndex = 1
 
        if(currentIndex > 11) currentIndex = 11
 
        document.getElementById("image").setAttribute("src", 'images/'+ currentIndex + ".png")
    }
 
</script>
 
