<p align="center">
<a href="https://pi-hole.net"><img src="https://pi-hole.github.io/graphics/Vortex/Vortex_with_text.png" width="150" height="255" alt="Pi-hole"></a>
<br/><br/>
<b>Network-wide ad blocking via your own Linux hardware</b><br/>
</p>

The Pi-hole[®](https://pi-hole.net/trademark-rules-and-brand-guidelines/) is a [DNS sinkhole](https://en.wikipedia.org/wiki/DNS_Sinkhole) that protects your devices from unwanted content, without installing any client-side software.

## Documentation & User Guides

This repo is the source for the official [Pi-hole documentation](https://docs.pi-hole.net/).

### How to contribute.
To add a new link on the navigation panel you need to edit the `mkdocs.yml` file in the root of the repo. There is a guide for building the navbar [on the mkdocs wiki]( https://www.mkdocs.org/user-guide/configuration/#nav)

To add a new document or guide.

- Navigate to the directory where it will be hosted.
	EG. guides are in `docs/guides`
- Create the file using a URL friendly filename.
	EG. `docs/guides/url-friendly.md`
- Edit your document using Markdown, there are loads of resources available for the correct syntax.


### Testing your changes.
Whilst working on this repo, it is advised that you review your own changes locally before commiting them. The `mkdocs serve` command can be used to live preview your changes (as you type) on your local machine.

Please make sure you fork the repo and change the clone URL in the example below for your fork:

- Linux Mint / Ubuntu instructions (tested on Linux Mint 18):
   - Preparations (only required once):
   ```bash
   git clone https://github.com/YOUR-USERNAME/docs
   cd docs
   sudo pip install mkdocs
   sudo pip install mkdocs-material markdown-include
   ```
   - Running the docs server:
   ```bash
   mkdocs serve --dev-addr 0.0.0.0:8000
   ```

- Fedora Linux instructions (tested on Fedora Linux 28):
   - Preparations (only required once):
   ```bash
   git clone https://github.com/YOUR-USERNAME/docs
   cd docs
   pip install mkdocs --user
   pip install mkdocs-material markdown-include --user
   ```
   - Running the docs server:
   ```bash
   mkdocs serve --dev-addr 0.0.0.0:8000
   ```

After these commands, the currently checked out branch is accessible through your favorite browser at http://localhost:8000
