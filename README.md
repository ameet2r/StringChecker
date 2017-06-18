## String Checker

<p>
    Please input the two strings you want to double check:
</p>

<!--Grab maze width and height from user-->
Maze Width: <input type="text" name="string1" value="5" id="string1">
<br>
Maze Height: <input type="text" name="string2" value="5" id="string2">
<br>
<input id="submitButton" type="submit" value="Submit" onclick="checkStrings()">

<p id="output">Result: </p>

<script>
    function checkStrings() {
        var string1 = document.getElementById("string1").value;
        var string2 = document.getElementById("string2").value;

        if(string1 === string2) {
            document.getElementById("output").innerHTML = "Result: both strings are the same";
        } else {
            document.getElementById("output").innerHTML = "Result: the strings are not the same";
        }
    }
</script>
