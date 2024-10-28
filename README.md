@{
    ViewData["Title"] = "Home Page";
}

<h1 id="greeting"></h1>

<script>
    const message = "Good morning babe";
    let index = 0;

    function displayCharacter() {
        if (index < message.length) {
            document.getElementById("greeting").innerHTML += message.charAt(index);
            index++;
            setTimeout(displayCharacter, 500); // تأخير نصف ثانية
        }
    }

    displayCharacter();
</script>
