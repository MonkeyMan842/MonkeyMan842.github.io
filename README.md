### Don't know how or where to download vencord click the button below

<button onclick="window.location.href='vencord-setup.html'">Vencord Setup</button>
<br>
### Don't know how to import local or how to use online themes click the button below

<button onclick="window.location.href='add-themes'">test</button>
<br>
<br>
# Anime Themes
*All themes based on animes that I enjoy*

### My Dress-Up Darling 
this is a theme based on the anime My Dress-Up Darling
<br>
uses Yellow and Gold colors with an fan made image as the background slightly tinted
![Theme Preview](https://monkeyman842.github.io/ex-images/MDUD-ex.png)
<textarea id="MDUD-copy" style="display:none;">https://monkeyman842.github.io/themes/MDUD.theme.css</textarea>
<button onclick="copyToClipboard('MDUD-copy')">Copy MDUD Theme</button>
<textarea id="MDUD-download" style="display:none;">https://raw.githubusercontent.com/MonkeyMan842/MonkeyMan842.github.io/refs/heads/main/themes/MDUD.theme.css</textarea>
<button onclick="download('MDUD-download', 'MDUD.theme.css')">Download .css file</button>

### Frieren
this is a theme based on the anime Frieren: Beyond Journey's End
<br>
uses different shades of blue with a fan made image as the background tinted
![Theme Preview](https://monkeyman842.github.io/ex-images/Frieren-ex.png)
<textarea id="Frieren-copy" style="display:none;">https://monkeyman842.github.io/themes/Frieren.theme.css</textarea>
<button onclick="copyToClipboard('Frieren-copy')">Copy Frieren Theme</button>
<textarea id="Frieren-download" style="display:none;">https://raw.githubusercontent.com/MonkeyMan842/MonkeyMan842.github.io/refs/heads/main/themes/Frieren.theme.css</textarea>
<button onclick="download('Frieren-download', 'Frieren.theme.css')">Download .css file</button>
<br>
<br>
<br>
- - - - - - - -
# Friends Themes
*All themes I made for friends*

### Newscape
this is a theme for my friend Newscape
<br>
uses light blue and cyan with a Windows XP type of background slightly tinted
![Theme Preview](https://monkeyman842.github.io/ex-images/Newscape-ex.png)
<textarea id="Newscape-copy" style="display:none;">https://monkeyman842.github.io/themes/Newscape.theme.css</textarea>
<button onclick="copyToClipboard('Newscape-copy')">Copy Newscape's custom Theme</button>
<textarea id="Newscape-download" style="display:none;">https://raw.githubusercontent.com/MonkeyMan842/MonkeyMan842.github.io/refs/heads/main/themes/Newscape.theme.css</textarea>
<button onclick="download('Newscape-download', 'Newscape.theme.css')">Download .css file</button>



<script>
  //copy button fuction
  function copyToClipboard(id) {
    var text = document.getElementById(id).value;
    navigator.clipboard.writeText(text).then(function() {
      alert("Link copied!");
    });
  }
  
  //download button fuction
  async function download(id, fileName) {
  const fileUrl = document.getElementById(id).value;
  try {
    const response = await fetch(fileUrl);
    const blob = await response.blob();
    const url = window.URL.createObjectURL(blob);
    const link = document.createElement('a');
    link.href = url;
    link.setAttribute('download', fileName);
    document.body.appendChild(link);
    link.click();
    document.body.removeChild(link);
    window.URL.revokeObjectURL(url);
  } catch (error) {
    console.error("Download failed:", error);
    window.open(fileUrl, '_blank');
  }
}
</script>
