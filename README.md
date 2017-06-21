<p>
    Please input the two strings you want to double check:
</p>


String one: <input type="text" name="string1" value="5" id="string1">
<br>
String two: <input type="text" name="string2" value="5" id="string2">
<br>
<br>
<input id="submitButton" type="submit" value="Submit" onclick="checkStrings()">
<br>
<br>
Ignore case: <input id="ignoreCaseCheckBox" type="checkbox">

<p id="output">Result: </p>

<script>
    function checkStrings() {
        var string1 = document.getElementById("string1").value;
        var string2 = document.getElementById("string2").value;
        var ignoreCase = document.getElementById("ignoreCaseCheckBox").checked;
        console.log(ignoreCase);

        if(ignoreCase){
            console.log("ignoreCase true");
            string1 = string1.toUpperCase();
            string2 = string2.toUpperCase();
        }

        if(string1 === string2) {
            document.getElementById("output").innerHTML = "Result: both strings are the same";
        } else {
            document.getElementById("output").innerHTML = "Result: the strings are not the same";
        }
    }
</script>
