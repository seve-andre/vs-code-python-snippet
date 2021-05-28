<h1>Visual Studio Code User Snippets for Python</h1>
<p>
    Supports Mac/Windows/Linux Visual Studio Code!
    <a href="https://github.com/seve-andre/vs-code-python-snippet/blob/main/python.json"><strong>Go to json »</strong></a><br />
    All the snippet suggestions end with <strong>Py</strong>.
</p>
<h1>How to use</h1>
First things first, open Visual Studio Code and install <a href="https://marketplace.visualstudio.com/items?itemName=ms-python.python">Python</a> by Microsoft from the 
Extensions Marketplace.
<br />
<br />
Next follow these steps:
<br />
<ol>
  <li>Go to Manage (bottom left-gear icon) and click on User Snippets</li>
  <li>Delete the default file content</li>
  <li>Copy the json file from <a href="https://raw.githubusercontent.com/seve-andre/vs-code-python-snippet/main/python.json">here</a> with <strong>CTRL/CMD+A</strong>
  and then <strong>CTRL/CMD+C</strong></li>  
  <li>Paste the json file content on Visual Studio Code with <strong>CTRL/CMD+V</strong></li>
  <li>Save the file with <strong>CTRL/CMD+S</strong></li>
</ol>
<br />
Demonstration gif:
<img src="https://github.com/seve-andre/vs-code-python-snippet/blob/main/demonstration.gif" />
<h1>Better use</h1>
<ol>
  <li>Go to Manage (bottom left-gear icon) and click on Settings</li>
  <li>Search "snippet"</li>
  <li>Select <strong>top</strong> under Editor: Snippet Suggestions</li>  
  <li>Click on "Open Settings (JSON)" in the upper right hand corner of the settings page and add this: <br />
    <code>
    "[python]": {
        "editor.rulers": [79]
    }
    </code>
    <br />
    that adds the static vertical ruler, an unenforced right-side boundary, to follow PEP-8 (Python Style guide). <br />
    So, you shouldn't pass this line if you want to follow
    Python conventions for better readability
  </li>
    <li>I also suggest adding these <strong>(Remember adding "," after each instruction)</strong>:<br />
  <code>"code-runner.saveAllFilesBeforeRun": true</code><br />
  <code>"editor.formatOnSave": true</code><br />
  <code>"files.eol": "\n"</code>
  </li>
  <li>
    Go to <strong>Keyboard Shortcuts</strong> (always from the gear icon) and click on "Open Settings (JSON)" in the upper 
    right hand corner
  </li>
  <li>Search for "acceptSelectedSuggestion" command and change <strong>key</strong> from tab to enter. This will help you move
      better between <strong>placeholders</strong>
  </li>
  <li>
    If "acceptSelectedSuggestion" command is not present, add this to keybindings.json:<br />
    <code>{
        "key": "enter",
        "command": "acceptSelectedSuggestion",
        "when": "suggestWidgetVisible && textInputFocus"
    }</code>
  </li>
  
</ol>
Thank you for reading this. If you want, you can give me a star and a follow. You can find my profile 
<a href="https://github.com/seve-andre">here</a>
