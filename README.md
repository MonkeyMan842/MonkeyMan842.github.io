# Anime Themes
*All themes based on animes that I enjoy*

### My Dress-Up Darling 
this is a theme based on the anime My Dress-Up Darling
<br>
uses Yellow and Gold colors with an fan made image as the background slightly tinted
![Theme Preview](https://monkeyman842.github.io/ex-images/MDUD-ex.png)
<textarea id="theme1" style="display:none;">https://monkeyman842.github.io/themes/MDUD.theme.css</textarea>
<button onclick="copyToClipboard('theme1')">Copy MDUD Theme</button>
<textarea id="theme1-Download" style="display:none;">https://raw.githubusercontent.com/MonkeyMan842/MonkeyMan842.github.io/refs/heads/main/themes/MDUD.theme.css</textarea>
<button onclick="download('theme1-Download', 'MDUD.theme.css')">Download .css file</button>

### Frieren
this is a theme based on the anime Frieren: Beyond Journey's End
<br>
uses different shades of blue with a fan made image as the background tinted
![Theme Preview](https://monkeyman842.github.io/ex-images/Frieren-ex.png)
<textarea id="theme2" style="display:none;">https://monkeyman842.github.io/themes/Frieren.theme.css</textarea>
<button onclick="copyToClipboard('theme2')">Copy Frieren Theme</button>
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
<textarea id="theme3" style="display:none;">https://monkeyman842.github.io/themes/Newscape.theme.css</textarea>
<button onclick="copyToClipboard('theme3')">Copy Newscape's custom Theme</button>



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
    // 1. Fetch the data from GitHub
    const response = await fetch(fileUrl);
    const blob = await response.blob();
    
    // 2. Create a local "Object URL" for that data
    const url = window.URL.createObjectURL(blob);
    
    // 3. Create the ghost link using the local URL
    const link = document.createElement('a');
    link.href = url;
    link.setAttribute('download', fileName);
    document.body.appendChild(link);
    
    // 4. Trigger the save-to-disk
    link.click();
    
    // 5. Cleanup
    document.body.removeChild(link);
    window.URL.revokeObjectURL(url);
    
    alert("Download started!");
  } catch (error) {
    console.error("Download failed:", error);
    // If something goes wrong, it will at least open the raw file
    window.open(fileUrl, '_blank');
  }
}
</script>


### Don't know how or where to download vencord and use its Themes click the link below

<button onclick="window.location.href='vencord-setup.html'">Vencord setup</button>
