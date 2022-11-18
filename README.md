# Python para executável em programas mais complexos
<div>
<img src="http://img.shields.io/static/v1?label=STATUS&message=%20FINALIZADO&color=GREEN&style=for-the-badge"/>
</div>
<div>
<a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/f06aea2585a5ebb7c97ff88c1e3ec42fe92502fbd897abe4bf2e56eb7039e1aa/68747470733a2f2f63646e2e69636f6e2d69636f6e732e636f6d2f69636f6e73322f3131322f504e472f3531322f707974686f6e5f31383839342e706e67"><img src="https://camo.githubusercontent.com/f06aea2585a5ebb7c97ff88c1e3ec42fe92502fbd897abe4bf2e56eb7039e1aa/68747470733a2f2f63646e2e69636f6e2d69636f6e732e636f6d2f69636f6e73322f3131322f504e472f3531322f707974686f6e5f31383839342e706e67" alt="python" width="40" height="40" data-canonical-src="https://cdn.icon-icons.com/icons2/112/PNG/512/python_18894.png" style="max-width: 100%;"></a></p>
</div>

### Objetivo:

Muitas vezes nossos códigos puxam informações de outros arquivos ou, no caso de webscraping, usam outros arquivos como o chromedriver.exe para funcionar.

Nesses casos, precisamos não só tomar alguns cuidados, mas também adaptar o nosso código para funcionar.

### O que usaremos:

- auto-py-to-exe para transformar o arquivo python em executável
- pathlib ou os para adaptar todos os "caminhos dos arquivos"
- Alternativamente, podemos usar o tkinter que nos permiti escolher manualmente o arquivo, independente do computador que vamos rodar o programa

- Referências Úteis:
    1. https://dev.to/eshleron/how-to-convert-py-to-exe-step-by-step-guide-3cfi
    2. https://pypi.org/project/auto-py-to-exe/


<div data-target="readme-toc.content" class="Box-body px-5 pb-5">
            <article class="markdown-body entry-content container-lg" itemprop="text"><h1 align="center" dir="auto"><a id="user-content-auto-py-to-exe" class="anchor" aria-hidden="true" href="#auto-py-to-exe"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Auto PY to EXE</h1>
<p align="center" dir="auto">A .py to .exe converter using a simple graphical interface and <a href="https://pyinstaller.readthedocs.io/en/stable/index.html" rel="nofollow">PyInstaller</a> in Python.</p>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/f28d9381fb102478b58e01da316b2259e9a0d7c800bbd1ca0ab1aa615eafcabd/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f666561747572652e706e67"><img src="https://camo.githubusercontent.com/f28d9381fb102478b58e01da316b2259e9a0d7c800bbd1ca0ab1aa615eafcabd/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f666561747572652e706e67" alt="Empty interface" data-canonical-src="https://nitratine.net/posts/auto-py-to-exe/feature.png" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto">
    <a href="https://pypi.org/project/auto-py-to-exe/" rel="nofollow"><img src="https://camo.githubusercontent.com/a61d2b2f44526d82af21ab60a9242efa7dc3c04db46295366a1a152ca6a65c99/68747470733a2f2f696d672e736869656c64732e696f2f707970692f762f6175746f2d70792d746f2d6578652e737667" alt="PyPI Version" data-canonical-src="https://img.shields.io/pypi/v/auto-py-to-exe.svg" style="max-width: 100%;"></a>
    <a href="https://pypi.org/project/auto-py-to-exe/" rel="nofollow"><img src="https://camo.githubusercontent.com/0af5f358d88f22f6ad5824ec9b0fb241a036f09d8e848f24ca274b2469d71497/68747470733a2f2f696d672e736869656c64732e696f2f707970692f707976657273696f6e732f6175746f2d70792d746f2d6578652e737667" alt="PyPI Supported Versions" data-canonical-src="https://img.shields.io/pypi/pyversions/auto-py-to-exe.svg" style="max-width: 100%;"></a>
    <a href="https://pypi.org/project/auto-py-to-exe/" rel="nofollow"><img src="https://camo.githubusercontent.com/1bb009d1d8b18d1c52fa8e721d1945d072ae04bdb26ac30586075be8008e6516/68747470733a2f2f696d672e736869656c64732e696f2f707970692f6c2f6175746f2d70792d746f2d6578652e737667" alt="License" data-canonical-src="https://img.shields.io/pypi/l/auto-py-to-exe.svg" style="max-width: 100%;"></a>
    <a href="https://pepy.tech/project/auto-py-to-exe" rel="nofollow"><img src="https://camo.githubusercontent.com/dd45e1a848f440e8c88b0cf74058d4dc2aaa4d0fcce99eae448351ff3bb8b1b6/68747470733a2f2f7374617469632e706570792e746563682f62616467652f6175746f2d70792d746f2d6578652f6d6f6e7468" alt="Downloads Per Month" data-canonical-src="https://static.pepy.tech/badge/auto-py-to-exe/month" style="max-width: 100%;"></a>
    <a href="https://pyinstaller.readthedocs.io/en/stable/requirements.html" rel="nofollow"><img src="https://camo.githubusercontent.com/8348e7ea36dbbe6c784542d9ac9b43a7ed55c001884a6cd07a01020cf586e666/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f706c6174666f726d2d77696e646f77732532302537432532306c696e75782532302537432532306d61636f732d6c6967687467726579" alt="Supported Platforms" data-canonical-src="https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-lightgrey" style="max-width: 100%;"></a>
    <a href="https://www.buymeacoffee.com/brentvollebregt" rel="nofollow"><img src="https://camo.githubusercontent.com/be2a5c5c104640151dfe9e2a215e050ae582e48e59594ac3df7ea6912b3bd97e/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f2d6275795f6d655f61254332254130626565722d677261793f6c6f676f3d6275792d6d652d612d636f66666565" alt="Donate" data-canonical-src="https://img.shields.io/badge/-buy_me_a%C2%A0beer-gray?logo=buy-me-a-coffee" style="max-width: 100%;"></a>
</p>
<p dir="auto">阅读中文版的README ，点击 <a href="/brentvollebregt/auto-py-to-exe/blob/master/README-Chinese.md">这里</a></p>
<h2 dir="auto"><a id="user-content-demo" class="anchor" aria-hidden="true" href="#demo"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Demo</h2>
<p align="center" dir="auto">
    <animated-image data-catalyst=""><a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/a0bb164ee9cfc14e26ee7840710c2d04237657c48c7646e335a07055324a8b54/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f6175746f2d70792d746f2d6578652d64656d6f2e676966" data-target="animated-image.originalLink"><img src="https://camo.githubusercontent.com/a0bb164ee9cfc14e26ee7840710c2d04237657c48c7646e335a07055324a8b54/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f6175746f2d70792d746f2d6578652d64656d6f2e676966" alt="auto-py-to-exe Demo" data-canonical-src="https://nitratine.net/posts/auto-py-to-exe/auto-py-to-exe-demo.gif" style="max-width: 100%; display: inline-block;" data-target="animated-image.originalImage"></a>
      <span class="AnimatedImagePlayer" data-target="animated-image.player" hidden="">
        <a data-target="animated-image.replacedLink" class="AnimatedImagePlayer-images" href="https://camo.githubusercontent.com/a0bb164ee9cfc14e26ee7840710c2d04237657c48c7646e335a07055324a8b54/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f6175746f2d70792d746f2d6578652d64656d6f2e676966" target="_blank">
          <span data-target="animated-image.imageContainer">
            <img data-target="animated-image.replacedImage" alt="auto-py-to-exe Demo" class="AnimatedImagePlayer-animatedImage" src="https://camo.githubusercontent.com/a0bb164ee9cfc14e26ee7840710c2d04237657c48c7646e335a07055324a8b54/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f6175746f2d70792d746f2d6578652d64656d6f2e676966" style="display: block; opacity: 1;">
          <canvas class="AnimatedImagePlayer-stillImage" aria-hidden="true" width="630" height="661"></canvas></span>
        </a>
        <button data-target="animated-image.imageButton" class="AnimatedImagePlayer-images" tabindex="-1" aria-label="Play auto-py-to-exe Demo"></button>
        <span class="AnimatedImagePlayer-controls" data-target="animated-image.controls">
          <button data-target="animated-image.playButton" class="AnimatedImagePlayer-button" aria-label="Play auto-py-to-exe Demo">
            <svg aria-hidden="true" focusable="false" class="octicon icon-play" width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M4 13.5427V2.45734C4 1.82607 4.69692 1.4435 5.2295 1.78241L13.9394 7.32507C14.4334 7.63943 14.4334 8.36057 13.9394 8.67493L5.2295 14.2176C4.69692 14.5565 4 14.1739 4 13.5427Z">
            </path></svg>
            <svg aria-hidden="true" focusable="false" class="octicon icon-pause" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
              <rect x="4" y="2" width="3" height="12" rx="1"></rect>
              <rect x="9" y="2" width="3" height="12" rx="1"></rect>
            </svg>
          </button>
          <a data-target="animated-image.openButton" aria-label="Open auto-py-to-exe Demo in new window" class="AnimatedImagePlayer-button" href="https://camo.githubusercontent.com/a0bb164ee9cfc14e26ee7840710c2d04237657c48c7646e335a07055324a8b54/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f6175746f2d70792d746f2d6578652d64656d6f2e676966" target="_blank">
            <svg aria-hidden="true" class="octicon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="16" height="16">
              <path fill-rule="evenodd" d="M10.604 1h4.146a.25.25 0 01.25.25v4.146a.25.25 0 01-.427.177L13.03 4.03 9.28 7.78a.75.75 0 01-1.06-1.06l3.75-3.75-1.543-1.543A.25.25 0 0110.604 1zM3.75 2A1.75 1.75 0 002 3.75v8.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 12.25v-3.5a.75.75 0 00-1.5 0v3.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-8.5a.25.25 0 01.25-.25h3.5a.75.75 0 000-1.5h-3.5z"></path>
            </svg>
          </a>
        </span>
      </span></animated-image>
</p>
<h2 dir="auto"><a id="user-content-getting-started" class="anchor" aria-hidden="true" href="#getting-started"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Getting Started</h2>
<h3 dir="auto"><a id="user-content-prerequisites" class="anchor" aria-hidden="true" href="#prerequisites"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Prerequisites</h3>
<ul dir="auto">
<li>Python : 3.6-3.11</li>
</ul>
<p dir="auto"><em>To have the interface displayed in the images, you will need chrome. If chrome is not installed or --no-chrome is supplied, the default browser will be used.</em></p>
<blockquote>
<p dir="auto">As of <a href="https://github.com/pyinstaller/pyinstaller/releases/tag/v4.0">PyInstaller 4.0</a>, Python 2.7 is no longer supported. Read "<a href="#python-27-support">Python 2.7 Support</a>" below for steps on how to use this tool with Python 2.7.</p>
</blockquote>
<h3 dir="auto"><a id="user-content-installation-and-usage" class="anchor" aria-hidden="true" href="#installation-and-usage"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Installation and Usage</h3>
<h4 dir="auto"><a id="user-content-installing-via-pypi" class="anchor" aria-hidden="true" href="#installing-via-pypi"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Installing Via <a href="https://pypi.org/project/auto-py-to-exe/" rel="nofollow">PyPI</a></h4>
<p dir="auto">You can install this project using PyPI:</p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ pip install auto-py-to-exe
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ pip install auto-py-to-exe" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">Then to run it, execute the following in the terminal:</p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ auto-py-to-exe
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ auto-py-to-exe" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h3 dir="auto"><a id="user-content-installing-via-github" class="anchor" aria-hidden="true" href="#installing-via-github"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Installing Via <a href="https://github.com/brentvollebregt/auto-py-to-exe">GitHub</a></h3>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ git clone https://github.com/brentvollebregt/auto-py-to-exe.git
$ cd auto-py-to-exe
$ python setup.py install
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ git clone https://github.com/brentvollebregt/auto-py-to-exe.git
$ cd auto-py-to-exe
$ python setup.py install" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto">Then to run it, execute the following in the terminal:</p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ auto-py-to-exe
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ auto-py-to-exe" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h4 dir="auto"><a id="user-content-running-locally-via-github-no-install" class="anchor" aria-hidden="true" href="#running-locally-via-github-no-install"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Running Locally Via <a href="https://github.com/brentvollebregt/auto-py-to-exe">Github</a> (no install)</h4>
<p dir="auto">You can run this project locally by following these steps:</p>
<ol dir="auto">
<li>Clone/download the <a href="https://github.com/brentvollebregt/auto-py-to-exe">repo</a></li>
<li>Open cmd/terminal and cd into the project</li>
<li>Execute <code>python -m pip install -r requirements.txt</code></li>
</ol>
<p dir="auto">Now to run the application, execute <code>python -m auto_py_to_exe</code>. A Chrome window in app mode will open with the project running inside.</p>
<blockquote>
<p dir="auto">Make sure you are in the directory below auto_py_to_exe (you will be after step 3) when calling <code>python -m auto_py_to_exe</code> or you will need to reference the folder auto_py_to_exe absolutely/relatively to where you currently are.</p>
</blockquote>
<h2 dir="auto"><a id="user-content-using-the-application" class="anchor" aria-hidden="true" href="#using-the-application"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Using the Application</h2>
<ol dir="auto">
<li>Select your script location (paste in or use a file explorer)
<ul dir="auto">
<li>Outline will become blue when file exists</li>
</ul>
</li>
<li>Select other options and add things like an icon or other files</li>
<li>Click the big blue button at the bottom to convert</li>
<li>Find your converted files in /output when completed</li>
</ol>
<p dir="auto"><em>Easy.</em></p>
<h3 dir="auto"><a id="user-content-arguments" class="anchor" aria-hidden="true" href="#arguments"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Arguments</h3>
<p dir="auto">Usage: <code>auto-py-to-exe [-nc] [-c [CONFIG]] [-o [PATH]] [filename]</code></p>
<table>
<thead>
<tr>
<th>Argument</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>filename</td>
<td>positional/optional</td>
<td>Pre-fill the "Script Location" field in the UI.</td>
</tr>
<tr>
<td>-nc, --no-chrome</td>
<td>optional</td>
<td>Open the UI using the default browser (which may be Chrome). Will not try to find Chrome.</td>
</tr>
<tr>
<td>-nu, --no-ui</td>
<td>optional</td>
<td>Don't try to open the UI in a browser and simply print out the address that the application can be accessed at.</td>
</tr>
<tr>
<td>-c [CONFIG], --config [CONFIG]</td>
<td>optional</td>
<td>Provide a configuration file (json) to pre-fill the UI. These can be generated in the settings tab.</td>
</tr>
<tr>
<td>-o [PATH], --output-dir [PATH]</td>
<td>optional</td>
<td>Set the default output directory. This can still be changed in the ui.</td>
</tr>
<tr>
<td>-bdo [FOLDER_PATH], --build-directory-override [FOLDER_PATH]</td>
<td>optional</td>
<td>Override the default build directory. Useful if you need to whitelist a folder to stop your antivirus from removing files.</td>
</tr>
<tr>
<td>-lang [LANGUAGE_CODE], --language [LANGUAGE_CODE]</td>
<td>optional</td>
<td>Hint the UI what language it should default to when opening. Language codes can be found in the table under "Translations" below.</td>
</tr>
</tbody>
</table>
<blockquote>
<p dir="auto">If you are running this package locally, you will need to call <code>python -m auto_py_to_exe</code> instead of <code>auto-py-to-exe</code></p>
</blockquote>
<h3 dir="auto"><a id="user-content-json-configuration" class="anchor" aria-hidden="true" href="#json-configuration"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>JSON Configuration</h3>
<p dir="auto">Instead of inserting the same data into the UI over and over again, you can export the current state by going to the "Configuration" section within the settings tab and exporting the config to a JSON file. This can then be imported into the UI again to re-populate all fields.</p>
<p dir="auto">This JSON config export action does not save the output directory automatically as moving hosts could mean different directory structures. If you want to have the output directory in the JSON config, add the directory under <code>nonPyinstallerOptions.outputDirectory</code> in the JSON file (will need to create a new key).</p>
<h2 dir="auto"><a id="user-content-video" class="anchor" aria-hidden="true" href="#video"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Video</h2>
<p dir="auto">If you need something visual to help you get started, <a href="https://youtu.be/OZSZHmWSOeM" rel="nofollow">I made a video for the original release of this project</a>; some things may be different but the same concepts still apply.</p>
<h2 dir="auto"><a id="user-content-issues-using-the-tool" class="anchor" aria-hidden="true" href="#issues-using-the-tool"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Issues Using the Tool</h2>
<p dir="auto">If you're having issues with the packaged executable or using this tool in general, I recommend you read <a href="https://nitratine.net/blog/post/issues-when-using-auto-py-to-exe/?utm_source=auto_py_to_exe&amp;utm_medium=readme_link&amp;utm_campaign=auto_py_to_exe_help" rel="nofollow">my blog post on common issues when using auto-py-to-exe</a>. This post covers things you should know about packaging Python scripts and fixes for things that commonly go wrong.</p>
<h2 dir="auto"><a id="user-content-translations" class="anchor" aria-hidden="true" href="#translations"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Translations</h2>
<table>
<thead>
<tr>
<th>Language</th>
<th>Code</th>
<th>Translator</th>
<th>Translated</th>
</tr>
</thead>
<tbody>
<tr>
<td>Arabic (العربية)</td>
<td>ar</td>
<td><a href="https://github.com/tayeb-ali">Tayeb-Ali</a></td>
<td>UI</td>
</tr>
<tr>
<td>Brazilian Portuguese (Português Brasileiro)</td>
<td>pt_br</td>
<td><a href="https://github.com/marleyas">marleyas</a></td>
<td>UI (partial)</td>
</tr>
<tr>
<td>Chinese Simplified (简体中文)</td>
<td>zh</td>
<td><a href="https://github.com/jiangzhe11">jiangzhe11</a></td>
<td>UI and <a href="/brentvollebregt/auto-py-to-exe/blob/master/README-Chinese.md">README</a></td>
</tr>
<tr>
<td>Chinese Traditional (繁體中文)</td>
<td>zh_tw</td>
<td><a href="https://github.com/ystartgo">startgo</a></td>
<td>UI</td>
</tr>
<tr>
<td>Czech</td>
<td>cz</td>
<td><a href="https://github.com/Matto58">Matto58</a></td>
<td>UI</td>
</tr>
<tr>
<td>English</td>
<td>en</td>
<td>-</td>
<td>UI and README</td>
</tr>
<tr>
<td>French (Français)</td>
<td>fr</td>
<td><a href="https://github.com/flaviedesp">flaviedesp</a></td>
<td>UI</td>
</tr>
<tr>
<td>German (Deutsch)</td>
<td>de</td>
<td><a href="https://github.com/hebens">hebens</a></td>
<td>UI (partial)</td>
</tr>
<tr>
<td>Greek (Ελληνικά)</td>
<td>gr</td>
<td><a href="https://github.com/sofronas">sofronas</a></td>
<td>UI</td>
</tr>
<tr>
<td>Indonesian (Bahasa Indonesia)</td>
<td>id</td>
<td><a href="https://github.com/MarvinZhong">MarvinZhong</a></td>
<td>UI</td>
</tr>
<tr>
<td>Italian (Italiano)</td>
<td>it</td>
<td><a href="https://github.com/itsEmax64">itsEmax64</a></td>
<td>UI</td>
</tr>
<tr>
<td>Russian (Русский)</td>
<td>ru</td>
<td>Oleg</td>
<td>UI</td>
</tr>
<tr>
<td>Spanish (Español)</td>
<td>sp</td>
<td><a href="https://github.com/enriiquee">enriiquee</a></td>
<td>UI</td>
</tr>
<tr>
<td>Thai (ภาษาไทย)</td>
<td>th</td>
<td><a href="https://github.com/teerut26">teerut26</a></td>
<td>UI (partial)</td>
</tr>
<tr>
<td>Turkish (Türkçe)</td>
<td>tr</td>
<td><a href="https://github.com/mcagriaksoy">mcagriaksoy</a></td>
<td>UI</td>
</tr>
</tbody>
</table>
<blockquote>
<p dir="auto">Want to add a translation for another language? Update <a href="https://github.com/brentvollebregt/auto-py-to-exe/blob/master/auto_py_to_exe/web/js/i18n.js">i18n.js</a> and submit a PR or attach it in an issue.</p>
</blockquote>
<h2 dir="auto"><a id="user-content-python-27-support" class="anchor" aria-hidden="true" href="#python-27-support"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Python 2.7 Support</h2>
<p dir="auto">As of <a href="https://github.com/pyinstaller/pyinstaller/releases/tag/v4.0">PyInstaller v4.0</a> released on Aug 9 2020, Python 2.7 is no longer supported; although you can still use this tool with Python 2.7 by installing an older version of PyInstaller. <a href="https://github.com/pyinstaller/pyinstaller/releases/tag/v3.6">PyInstaller v3.6</a> was the last version that supported Python 2.7; to install this, first uninstall any existing versions of PyInstaller and then execute <code>python -m pip install pyinstaller==3.6</code>.</p>
<h2 dir="auto"><a id="user-content-testing" class="anchor" aria-hidden="true" href="#testing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Testing</h2>
<p dir="auto">Tests are located in <code>tests/</code> and are run using pytest:</p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>$ pip install pytest
$ pip install -e .
$ pytest
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="$ pip install pytest
$ pip install -e .
$ pytest" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 dir="auto"><a id="user-content-screenshots" class="anchor" aria-hidden="true" href="#screenshots"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Screenshots</h2>
<table>
<thead>
<tr>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://nitratine.net/posts/auto-py-to-exe/empty-interface.png" rel="nofollow"><img src="https://camo.githubusercontent.com/4c3ef7d7a81d722754edf16ad09c7713d42ffd44fb0b7e33d953c9c96fcea4d1/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f656d7074792d696e746572666163652e706e67" alt="Empty interface" data-canonical-src="https://nitratine.net/posts/auto-py-to-exe/empty-interface.png" style="max-width: 100%;"></a></td>
<td><a href="https://nitratine.net/posts/auto-py-to-exe/filled-out.png" rel="nofollow"><img src="https://camo.githubusercontent.com/c610267f3a63e48347a40acfcb5d8d00517b2ac81eb4c6cf0805fd8ff5ae5068/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f66696c6c65642d6f75742e706e67" alt="Filled out" data-canonical-src="https://nitratine.net/posts/auto-py-to-exe/filled-out.png" style="max-width: 100%;"></a></td>
</tr>
<tr>
<td><a href="https://nitratine.net/posts/auto-py-to-exe/converting.png" rel="nofollow"><img src="https://camo.githubusercontent.com/ee5000efacbcfa537713e09d7aa91b0173374c0d0b54afa9dee97dc906ada73f/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f636f6e76657274696e672e706e67" alt="Converting" data-canonical-src="https://nitratine.net/posts/auto-py-to-exe/converting.png" style="max-width: 100%;"></a></td>
<td><a href="https://nitratine.net/posts/auto-py-to-exe/completed.png" rel="nofollow"><img src="https://camo.githubusercontent.com/38b0a4aec8e29617306a7dccb1a42b5abcc7e2c2cbe7ace31b83dcd69e8b0108/68747470733a2f2f6e6974726174696e652e6e65742f706f7374732f6175746f2d70792d746f2d6578652f636f6d706c657465642e706e67" alt="Completed" data-canonical-src="https://nitratine.net/posts/auto-py-to-exe/completed.png" style="max-width: 100%;"></a></td>
</tr>
</tbody>
</table>
</article>
          </div>
