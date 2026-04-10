# Anime Themes
*All themes based on animes that I enjoy*

### My Dress-Up Darling 
this is a theme based on the anime My Dress-Up Darling
<br>
uses Yellow and Gold colors with an fan made image as the background slightly darkend
![Theme Preview](https://monkeyman842.github.io/ex-images/MDUD-ex.png)
<textarea id="theme1" style="display:none;">https://monkeyman842.github.io/themes/MDUD.theme.css</textarea>
<button onclick="copyToClipboard('theme1')">Copy MDUD Theme</button>

### Frieren
this is a theme based on the anime Frieren: Beyond Journey's End
<br>
uses different shades of blue with a fan made image as the background darkend
![Theme Preview](https://monkeyman842.github.io/ex-images/Frieren-ex.png)
<textarea id="theme2" style="display:none;">https://monkeyman842.github.io/themes/Frieren.theme.css</textarea>
<button onclick="copyToClipboard('theme2')">Copy Frieren Theme</button>

<textarea id="theme3" style="display:none;">https://monkeyman842.github.io/themes/Newscape.theme.css</textarea>
<button onclick="copyToClipboard('theme3')">Copy Newscape's custom Theme</button>



<script>
  function copyToClipboard(id) {
    var text = document.getElementById(id).value;
    navigator.clipboard.writeText(text).then(function() {
      alert("Link copied!");
    });
  }
</script>
