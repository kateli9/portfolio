# Kate Li’s portfolio

This static site runs without a build step. The repository root opens Published (`index.html`); the header also links to `projects.html`. To preview both pages locally, run `python3 -m http.server 8000` from the repository root and open `http://localhost:8000/`.

Edit the `bio` paragraph in `index.html` to add your introduction. Each category contains one or more `<article class="work-entry">` blocks. Replace the title, description, and the two `<dd>` values for time and skills. Copy or remove a block to adjust the number of entries. The same markup can be used for previous work in `projects.html`.

Save article graphics in `assets/` and replace the `artwork-placeholder` element with an image. Give the image alt text that describes what it shows. The square frame displays the whole graphic.

```html
<img class="artwork" src="assets/article-graphic.png"
     alt="Describe the graphic here" loading="lazy">
```

Replace each link placeholder with a real link inside `work-links`. Add more article links as needed and include the GitHub link only when there’s a repository to share.

```html
<div class="work-links">
  <a href="https://example.com/article">
    <img src="assets/arrow-up-right.svg" alt="" width="16" height="16">
    Read the article
  </a>
  <a href="https://github.com/owner/repository">
    <img src="assets/github.svg" alt="" width="16" height="16">
    View on GitHub
  </a>
</div>
```
