# obadah.github.io

Personal academic website, built with Jekyll and served by GitHub Pages (no theme, no build step needed).

## Editing content

| What | Where |
| --- | --- |
| Name, email, profile links | `_config.yml` (`author:`) |
| Bio and home page | `index.md` |
| News items | `_data/news.yml` |
| Publications | `_data/publications.yml` |
| Writing / blog posts | `_posts/YYYY-MM-DD-title.md` |
| CV page | `cv.md`; drop the PDF at `assets/cv.pdf` |
| Styles | `assets/css/style.css` |

## Local preview

```sh
bundle install
bundle exec jekyll serve
```
