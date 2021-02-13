# ox-hugo-blog-content
The org-mode based setup for blogging at Emacs-SF.github.io

## blog post author pre-reqs:
1. install hugo on your system
2. configure ox-hugo in your emacs
3. fork this repository
4. clone your fork using --recursive to get the theme git submodule

## blog post author worflow:
1. create or edit some-unique-post.org file in org-content/posts; add images to same directory if desired
(look at existing post for prolog lines to copy/edit)
2. use ox-hugo to export from org file to markdown file in content/posts
3. run hugo to generate index/categories/tags etc in public/ directory; use hugo server to test locally
4. git add/commit/push your changes to your fork
5. issue a pull request

## site maintainer pre-reqs:
1. install hugo
2. configure ox-hugo
3. clone this repo
4. clone the Emacs-SF.github.io repo under the same parent

## site maintainer workflow 
1. review/merge pull request
2. cp -pr public/* ../Emacs-SF.github.io # copy generated files to blog repo 
3. git add/commit/push changes to main branch; wait for [Emacs SF Blog site](https://emacs-sf.github.io/) to update - may take a minute or two
4. verify changes, new/changed post, new/changed category index/links if any, new/changed tag index/links if any
