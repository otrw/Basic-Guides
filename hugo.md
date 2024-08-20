# Hugo Basics Cheatsheet

## Installation
- Check [Hugo documentation](https://gohugo.io/installation/)

## Creating a New Site
- `hugo new site <site-name>`

## Theme Management
- `git clone <theme-repo> themes/<theme-name>`
- `git submodule add <theme-repo> themes/<theme-name>`
- Update `config.toml` to use the theme: `theme = "<theme-name>"`

## Content Creation
- `hugo new <section>/<file-name>.md`: Create a new content file
- `hugo new posts/my-first-post.md`: Example for a new blog post

## Development
- `hugo server`: Start the Hugo development server
- `hugo server -D`: Include draft content in development server

## Building Your Site
- `hugo`: Build your site (output to `public/` directory)
- `hugo --minify`: Build and minify your site

## Content Management
- Front matter: Add metadata at the top of content files
  ```yaml
  ---
  title: "My First Post"
  date: 2023-01-01T10:00:00-05:00
  draft: true
  ---
  ```

## Customization
- Edit `config.toml` for site-wide settings
- Create/edit layouts in `layouts/` directory
- Add static content (images, CSS, JS) to `static/` directory
- Templates for Posts stored in the `archetypes/` directory
## Useful Flags
- `-D` or `--buildDrafts`: Include draft content
- `-E` or `--buildExpired`: Include expired content
- `-F` or `--buildFuture`: Include content with future publish dates

## Help
- `hugo help`
- `hugo <command> --help`
- [official Hugo documentation](https://gohugo.io/documentation/).
