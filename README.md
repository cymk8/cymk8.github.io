# cymk8.github.io


## Pages

- `index.html`
  - Item listings grouped in horizontal tracks
- `all.html`
  - Listing of all items
  - Has filter based on title

## List Item Anatomy

```html
<li>
    <a href="https://cara.app/explore" target="_blank" class="lesson-item" data-title="Lesson 10 - Drawing">
        <img src="./images/icon.png" class="icon" alt="Lesson 10 - Drawing" />
        <span class="title">Lesson 10 - Drawing</span>
    </a>
</li>
```

The listing is basically in an unordered list (`<ul>`) and all the items are in each list item (`<li>`)

- The **url** goes in `href=""` attribute inside the `<a>` tag
  - This what where people are linked to
- The **title** goes in two places:
  - One inside the `data-title=""` attribute inside the `<a>` tag
    - This is for functionality purposes for the filter
  - One in between the `<span clas="title">` tags 
    - This is what gets displayed on the page
- The **image url** goes in the `src=""` attribute of the `<img>` tag
  - `alt` attribute is the image description for Accessibility


## Folder Structure

```
root (cymk8.github.io)
├── assets
│   ├── css.css
│   ├── css.scss
│   ├── js.js
│   └── override.css
├── images
│   └── images.png
├── all.html
└── index.html
```

- Styles
  -  `css.css` is compiled from `css.scss`
  - Use `override.css` for css if you can't compile/rebuild sass
- Function
  - `js.js` this is where js functionality is in
- Image
  - Images go in the images folder