---
title: "Mermaid commands"
---

# Command lines

## Installing Mermaid globally

```bash
npm install -g @mermaid-js/mermaid-cli
```

## Documentation and templates

Documentation and templates can be found here  
[link to documentation](https://mermaid.js.org/syntax/flowchart.html)

## Create diagrams from Mermaid code

**Generate \*.png files**

Raster image. Generate image to the Pixel

```bash
mmdc -i input.mmd -o output.png
```

**Generate \*.svg files**

Vector image. More compact but needs a specific package to include this image into .docx and .pdf files. Because `pandoc` has to convert this image into a raster image.

```bash
mmdc -i input.mmd -o output.svg
```

## Link images to the document

Once the .png and .svg files are generated, you can link the outside resources to the focument using the following MarkDown notation

```md
![Pythagoras Formula](Pythagore_V1.png)
```

You can also embed resources into the generated document by using the `--embed-resources` option.  

Example

```bash
pandoc your-document.md -o output.html --embed-resources
```

Note that yo also have the standalone option `-s` to generate a standalone document.

Example

```bash
pandoc your-document.md -s -o output.html
```

## Hot reload

Creating Mermaid diagrams on the fly with hot reload involves using tools that can watch for changes in your Mermaid code and automatically update the rendered diagram.

You can do this using  VS Code with Extensions and a File Watcher

- **VS Code Extensions**:
  - Install the "Mermaid Preview" extension (or a similar one) to get a preview pane within VS Code.
- **File Watcher** (e.g., chokidar-cli):
  - You can use a file watcher to detect changes in your .mmd files and then trigger a command to convert them to images or update a preview.
  - Install `chokidar-cli` globally: `npm install -g chokidar-cli`
  - Create a script that will render the mmd file, for example, a bash script or a node.js script.
  - Use `chokidar-cli` to watch for changes, and then execute your script.
  - Example using chokidar, and the mermaid cli:
    - `chokidar '*.mmd' -c 'mmdc -i {path} -o {path}.png'`
    - This will watch all .mmd files in the directory, and create .png files that have the same name.
  - You could then have an html file that refreshes the image every second.
