# ECEN 601 web lessons

`index.html` is the course landing page. After the repository's existing
GitHub Pages deployment, it is available at:

https://krntamu.github.io/ecen601/

The existing six HTML files stay in place to preserve their published URLs
and the links between the two SVD lessons.

## Adding topics

Use a folder per topic for new material. Use lowercase, hyphenated names,
and an `index.html` entry point for each topic:

```text
ecen601/
  index.html                  # Course landing page
  README.md                   # Authoring instructions
  fundamentalsubspaces.html   # Existing lessons retain their URLs
  svd.html
  svd-mathematics.html
  pca.html
  pagerank.html
  lagrange.html
  topics/
    least-squares/
      index.html              # /ecen601/topics/least-squares/
      assets/                 # Images, scripts, or data for this topic
    qr-decomposition/
      index.html
      assets/
  assets/                     # Only for files shared by multiple lessons
```

The `topics/` and `assets/` directories above are recommendations; create
them when you add material that needs them. Small standalone lessons can
keep their styles and scripts inline, as the existing pages do.

1. Create `topics/<topic-name>/index.html` with a descriptive title,
   viewport metadata, and a main heading.
2. Keep files used only by that topic in its own `assets/` folder. Reference
   them with relative URLs such as `assets/diagram.svg`.
3. Add a lesson card to the appropriate section's `<ul class="lessons">`
   in the landing page, linking to `topics/<topic-name>/`. Copy an existing
   `<li>` block and update its label, heading, description, and link.
4. Add a return link from the new topic to `../../` (the course landing page).
5. Check links locally, then commit and push through the repository's normal
   deployment workflow. Adding an HTML file alone does not add a landing-page card.

For multiple lessons on one topic, keep `index.html` as the topic overview
and put related pages beside it, for example `proof.html` or `examples.html`.
Group topics by subject on the landing page; avoid adding extra directory
levels until the amount of material calls for them.

No changes to `_config.yml` or a separate GitHub repository are needed for
this landing page. It is plain HTML, like the existing lesson files.
