# Github Heatmap Art

Want to show off some cool art on your GitHub contribution heatmap? You're in the right place

## Examples

![Example](https://github.com/Mindful-Developer/github_colourized_heatmap_chrome_ext/raw/main/imgs/before.png)


## How to use

Set up the [ocen](https://github.com/ocen-lang/ocen/) compiler on your machine. Additional requirements:
- For the image editor, you will need SDL installed and available on your default library path
- For uploading to GitHub, you will need to modify `process_image.oc` to include your GitHub username/email/repo URL. You will also need to set up your SSH keys for GitHub.

```
$ git clone https://github.com/mustafaquraish/gh-heatmap-art
$ cd gh-heatmap-art
$ ocen make_image.oc -r image.txt   # Create the image file
$ vim process_image.oc              # Change the Github user/repo info
$ ocen process_image.oc -r image.txt  --push  # Create the commits and push to GitHub
```

