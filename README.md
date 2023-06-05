
# QumaPage – Quasi-Markdown Page Generator

Markdown is great but limited. **QumaPage** is a small collection of addons for the Markdown converter [Pandoc](https://pandoc.org) to extend the possibilities of Markdown. In particular, QumaPage adds

* **True Multi-Output:** You can convert the same source file to `html`, `gfm`, or `pdf` and it will look great.
  * **[Math Support](#math-support):** You can typeset math in `tex` and it will be rendered for every output.
  * **[Icon Support](#fontawesome-unicode-icons-):** Use unicode icons that will be rendered with [FontAwesome](https://fontawesome.com/) when available and otherwise fallback to native icons.
  * **No Artefacts:** If a feature is not supported for one output type, it will not cause trouble but is rendered in a simpler form.
* **Additional Syntax:** 
  * **Inline Diagrams:** You can embedd code for diagrams in the `.md` and QumaPage will render the image. Currently, we support `matplotlib`, `ggplot`, `tikz`, `plantuml`
  * **Colored Boxes:** You can add boxes to seperate special content from the normal text flow.
  * **Collapse Details:** Hide additional info by default and reveal it only when the user clicks on it.
  * **Include Files:** You can include the content of other `.md` files.
* **Awesome HTML:** If the output is `html`, QumaPage will add bonus features to enhance readability.
  * **Dark Mode:** You can read the content in dark theme.
  * **Adjust Font Size:** You can increase or decrease the font size.
  * **Print Friendly:** Looks nice on A4 paper when printed.
  * **Heading Anchors:** automatic anchors at `h2` headings for one-click links.


## Getting Started
Only 4 small steps are required to build your first document.


1. Clone this repo
2. Install dependencies via `make setup`
3. open and edit `src/qmp-template.md`
4. build the file using `make` command (Unix)
5. open `build/qmp-template.html` in a browser

```bash
git clone git@github.com:emareg/qumapage.git
cd qumapage
make setup
xdg-open src/qmp-template.md
make
xdg-open build/qmp-template.html
```



