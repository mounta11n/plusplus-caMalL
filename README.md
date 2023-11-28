

<h1 align="center">Custom Frontend for llama.cpp Server</h1>

<br>
<br>


<p float="left">
  <img src="media/ui-1_chat.jpg" height="500" />
</p>



<br>
<h2 align="center">Features of this Frontend</h2>

<ul>
  <li><strong>User Interface.</strong> Designed with CSS for a more appealing and tidy appearance.</li>
  <li><strong>CSS-Auslagerung.</strong> The CSS has been moved to a separate file to simplify maintenance.</li>
  <li><strong>Dropdown-Menus.</strong> Drop-down menus for predefined prompt formats and system prompts have been added.</li>
  <li><strong>Modular structure.</strong> Prompt formats and system prompts are stored in separate files, which makes editing very easy.</li>
  <li><strong>More freedom.</strong> Prompt formats and system prompts are independent of each other and can therefore be combined as required.</li>
  <li><strong>Easy access for beginners.</strong> A script was created that utilizes "dialog" to compose the command for the server.</li>
  <li><strong>Configuration management.</strong> The script offers the option of saving and loading configurations.</li>
</ul>
<br>
<br>

<p float="right">
  <img src="media/tui-3_load-config.jpg" height="500" />
</p>

<br>
<br>
<br>
<h2 align="center">Planned functions</h2>

<ul>
  <li><strong>Multilingualism (in progress).</strong> It will be possible to select the language via a drop-down menu. So far, language files for English and German are available. Further languages will follow (support is welcome).</li>
  <li><strong>Dark mode.</strong> A dark mode for an eye-friendly view is currently in progress.</li>
  <li><strong>Low stimulus mode.</strong> A low-stimulus and low-contrast mode is being planned for people who need it.</li>
  <li><strong>Templates for UI options.</strong> Templates for the values of the user interface options (sampler etc.), such as deterministic template, creative template, balanced template etc., are planned.</li>
</ul>


<br>
<br>
<h2 align="center">How to start</h2>

<h3 align="left">Dialog Script</h3>

1. Wenn du dich mit `git clone` auskennst, muss ich dir den Prozess nicht erklären.

2. Solltest du dich mit git nicht auskennen, dann lade dir dieses Repository als ZIP Datei herunter: [Klick hier](https://github.com/mounta11n/plusplus-caMalL/archive/refs/heads/master.zip)


2. Entpacke die ZIP Datei und gehe daraufhin in den entpackten Ordner.

3. Finde eine Datei namens 'start-server.sh' und wähle die Datei mit der rechten Maustaste aus.

4. Gehe auf -> "öffnen mit" -> Terminal (iTerm, xterm, ..) – das war's

<br>
Das folgende Dialog-Fenster hilft dir, das Backend zu starten:

<br>
<br>

<p float="left">
  <img src="media/tui-1_main.jpg" height="400" />
  <img src="media/tui-2_options.jpg" width="400" />
</p>

<br>

<p float="right">
  <img src="media/tui-3_load-config.jpg" height="500" />
</p>

<br>
<br>

<h3 align="left">Zenity Script</h3>

<h6 align="left">Für den Fall, dass du Angst davor haben solltest, dich zu lange im Terminal aufzuhalten, gibt es auch für dich eine Lösung:</h6>

- Anstatt nach 'start-server.sh' zu suchen, suchst du nach 'zenity-server.sh'

- Die weiteren Schritte sind wie bei Dialog auszuführen.

- Dich wird folgendes Fenster begleiten:

<br>
<br>

<p float="left">
  <img src="media/gui-1_main.jpg" height="400" />
  <img src="media/gui-2_options.jpg" height="400" />
</p>

<br>
<br>

<h2 align="left">Some More Impressions</h2>



<br>
<br>
<h3 align="left">Docs</h3>

- [General Guide](https://github.com/ggerganov/llama.cpp#readme/)
- [main](./examples/main/README.md)
- [server](./examples/server/README.md)
- [jeopardy](./examples/jeopardy/README.md)
- [BLIS](./docs/BLIS.md)
- [Performance troubleshooting](./docs/token_generation_performance_tips.md)
- [GGML tips & tricks](https://github.com/ggerganov/llama.cpp/wiki/GGML-Tips-&-Tricks)
- [GBNF grammars](./grammars/README.md)
