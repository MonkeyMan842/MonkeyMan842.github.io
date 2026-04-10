<textarea id="theme1" style="display:none;">@import url('https://monkeyman842.github.io/cyberpunk.css');</textarea>
<button onclick="copyToClipboard('theme1')">Copy Cyberpunk Link</button>

<textarea id="theme2" style="display:none;">@import url('https://monkeyman842.github.io/midnight-discord.css');</textarea>
<button onclick="copyToClipboard('theme2')">Copy Midnight Link</button>

<script>
  function copyToClipboard(id) {
    var text = document.getElementById(id).value;
    navigator.clipboard.writeText(text).then(function() {
      alert("Link copied!");
    });
  }
</script>
