# Welcome to aosp-devs.org

aosp-devs is a community for AOSP Developers.

This repository contains the contents of the website [aosp-devs.org](https://aosp-devs.org).
Contributions are welcome. Feel free to open a PR.

## Run locally

```bash
docker run --rm \
  --name aosp-devs.org \
  -p 4000:4000 \
  -p 35729:35729 \
  -v "$PWD:/srv/jekyll" \
  -v "$PWD/vendor/bundle:/usr/local/bundle" \
  -it \
  jekyll/jekyll:4 \
  bash -lc 'bundle install && bundle exec jekyll serve --host 0.0.0.0 --livereload'
```

Open `http://127.0.0.1:4000`.
