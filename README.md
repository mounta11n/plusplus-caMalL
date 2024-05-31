<h1 align="center">Custom llama.cpp Frontend</h1>

**This is a fork, but it adresses only the the server and its web UI. This work will maybe become merged against the upstream. In that case this repo will eventually become to something like a playground for quick and dirty experiments and tinkerings, while the merged frontend at ggerganov/llama.cpp will be a stable and well maintained version**

<br>
<br>

<figure >
  <img src="media/ui-1_chat.jpg" width="800" />
  <figcaption>The Main Chat User Interface.</figcaption>
</figure>

<br>
<br>
<br>

<br>
<br>

<figure >
  <img src="media/mango-cpp.jpeg" width="800" />
  <figcaption>Dark Mango llama.cpp.</figcaption>
</figure>

<br>
<br>
<br>
<h2 align="center">Features of this Frontend</h2>

<br>

<ul>
  <li><strong>User Interface.</strong><br>Designed with CSS for a more appealing, clean and tidy appearance.</li><br>
  <li><strong>Well Known Style.</strong><br>My initial styling inspiration was the OpenAI playground. A lot of people are already used to this design. But in the meantime I have made some more color themes.</li><br>
  <li><strong>Dark and Light Themes.</strong><br>As mentioned, there are now some color themes to choose from.<br><br>
  <li><strong>CSS outsourcing.</strong><br>The CSS has been moved to separate files to simplify maintenance and hacking.</li><br>
  <li><strong>Dropdown-Menus.</strong><br>Convenient Drop-down menus for predefined prompt formats and system prompts have been added.</li><br>
  <li><strong>Modular structure.</strong><br>Prompt formats and system prompts are stored in separate files, which makes editing very easy.</li><br>
  <li><strong>More freedom.</strong><br>Prompt formats and system prompts are independent of each other and can therefore be combined as required.</li><br>
  <li><strong>Added a lot of tooltips.</strong><br>With comprehensible explanations regarding each parameter.</li><br>
  <li><strong>Easy access for beginners.</strong><br>A script was created that utilizes "dialog" to compose the command for the server.</li><br>
  <li><strong>Configuration management.</strong><br>The script offers the option of saving and loading configurations.</li>
</ul>
<br>
<br>

<figure>
  <img src="media/snowstorm.jpeg" width="800" />
  <figcaption>The new default UI</figcaption>
</figure>


[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Server](https://github.com/ggerganov/llama.cpp/actions/workflows/server.yml/badge.svg?branch=master&event=schedule)](https://github.com/ggerganov/llama.cpp/actions/workflows/server.yml)
[![Conan Center](https://shields.io/conan/v/llama-cpp)](https://conan.io/center/llama-cpp)
<br>
<br>
<br>
<br>


<br>
<br>

<figure>
  <img src="media/old-to-new.jpeg" width="800" />
  <figcaption>From the old UI just press on "New UI"</figcaption>
</figure>

<br>
<br>
<br>
<br>
<br>
<br>

<figure>
  <img src="media/polarnight.jpeg" width="800" />
  <figcaption>A very popular color theme: "Nord"</figcaption>
</figure>

<br>
<br>
<br>
<br>

<figure>
  <img src="media/ui-3_completion.jpg" width="800" />
  <figcaption>The Completion Interface. A Perfect Playground for Experimenting.</figcaption>
</figure>

<br>
<br>
<br>

<h2 align="center">Planned functions</h2>

<br>

<ul>
  <li><strong>Multilingualism (in progress).</strong><br>It will be possible to select the language via a drop-down menu. So far, language files for English and German are available. More languages will follow (support is welcome).</li><br>
  <li><del><strong>Dark mode.</strong><br>A dark mode for an eye-friendly view is currently in progress.</del></li><br>
  <li><strong>Low stimulus mode.</strong><br>A low-stimulus <del>and low-contrast</del> mode (not more after reading <a href="https://blog.pope.tech/2022/11/08/color-contrast-accessibility-requirements-explained/">this</a>) is being planned for people who need it.</li><br>
  <li><del><strong>Templates for UI options.</strong><br>Templates for the values of the user interface options (sampler etc.), such as deterministic template, creative template, balanced template etc., are planned.</del></li>
</ul>

<br>
<br>
<br>

<h2 align="center">Longterm Roadmap or "Wishes"</h2>

<br>

<ul>
  <li><strong>Speech to Text.</strong><br>Implement Interface for Whisper.cpp for STT</li><br>
  <li><strong>Vector Database.</strong><br>Implement Logic to Utilize Bert.cpp for efficient embeddings</li><br>
  <li><strong>Text to Speech.</strong><br>Waiting for a .cpp/ggml ecosystem TTS Solution ...</li><br>
  <li><strong>Extend UI.</strong><br>An additional View for Finetuning </li><br>
  <li><strong>Group-Chat.</strong><br>Simulated Multi- or Group-Chat </li>
</ul>

<br>

For those wishes I think I'll need some advices and help. Feel free to contact me if you're interested in working together on those things.


<br>
<br>
<br>

<h2 align="center">How to start</h2>

<br>
<br>
<br>

<h3 align="left">Build manually</h3>

1. Clone this repo<br>`git clone https://github.com/mounta11n/plusplus-camall.git && cd plusplus-camall`<br><br>
2. Make sure you are on the right branch, which is **not** master<br>`git switch plusplus`<br><br>
3. Compile the Server<br>`mkdir build && cd build`<br>`cmake ..`<br>`make server`<br><br>

<br>

<h3 align="left">Run the Server</h3>

1. `./bin/server -m /path/to/your/model.gguf`<br><br>

2. In your browser open `localhost:8080`
<br>
<br>
<br>
<br>

<h2 align="center">Some More Impressions</h2>

<br>
<br>
<br>

<h2 align="left">Further Options and Grammar</h2>
<br>
  <img src="media/ui-2_grammar.jpg" width="600" />

<br>
<br>
<br>

<h2 align="left">Prompt Formats</h2>
<br>
  <img src="media/prompt-formats.jpeg" width="600" />

<br>
<br>
<br>

<h2 align="left">System Prompts</h2>
<br>
  <img src="media/promptformat-sysprompt.png" width="600" />

<br>
<br>
<br>

<h2 align="left">UI Elements</h2>

<br>
<br>
<br>

<figure>
  <img src="media/ui-7_reset.jpg" width="800" />
  <figcaption></figcaption>
</figure>
<br>
<br>
<br>
<br>
<br>

<figure>
  <img src="media/text-select.png" width="800" />
  <figcaption>Crafted with attention to detail. Text selection adapts its color.</figcaption>
</figure>
<br>
<br>
<br>
<br>
<br>
<br>

<figure>
  <img src="media/hover-details.png" width="800" />
  <figcaption>Get more Info when you hover over the text.</figcaption>
</figure>

<br>
<br>
<br>
<br>

<h2 align="left">AI Response</h2>
<br>
  <img src="media/phi3-response.jpeg" width="600" />

<br>
<br>
<br>

<h2 align="left">Multimodality</h2>
<br>
  <img src="media/ui-9_multimodal.jpg" width="600" />

<br>
<br>
<br>


<h3 align="left">Docs</h3>

If you are looking for support, I would recommend to referr to the original llama.cpp, with first considering the following:


- [General Guide](https://github.com/ggerganov/llama.cpp#readme/)
- [main](./examples/main/README.md)
- [server](./examples/server/README.md)
- [Performance troubleshooting](./docs/token_generation_performance_tips.md)
- [GGML tips & tricks](https://github.com/ggerganov/llama.cpp/wiki/GGML-Tips-&-Tricks)
- [GBNF grammars](./grammars/README.md)
