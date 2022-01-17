# blog

[github-io]: https://devPalacio.github.io/blog
[bliss-new]: https://bliss.js.org/#/?o=devPalacio&r=blog&b=main&ght
[gh-settings-pages]: https://github.com/devPalacio/blog/settings/pages
[gh-actions]: https://github.com/devPalacio/blog/actions
[content-dir]: /content/blog/
[utterances-app]: https://github.com/apps/utterances
[gh-issues]: https://github.com/devPalacio/blog/issues

## Just a few steps to **Finish Up**:

## View Blog

You can view your blog at [devPalacio.github.io/blog][github-io].

<!--
  TODO edge case:
  https://devPalacio.github.io/devPalacio.github.io/
  is actually
  https://devPalacio.github.io/
-->

## New Post

<kbd><a href="https://bliss.js.org/#/?o=devPalacio&r=blog&b=main&ght">Create New Post</a></kbd>

You can make new blog posts as easy as Gists. Just write your ~~tweet~~ post,
and Bliss will fill out the Front Matter for you.

1. 🔎 Type <kbd>bli</kbd> in your browser's omnibar and hit <kbd>enter</kbd> (assuming you followed the steps above).
   - (or visit [bliss.js.org][bliss-new] directly)
2. 📝 Write your post
3. 💾 Click <kbd>Add to Github</kbd>, and then <kbd>Commit new file</kbd>

Your new post will build automatically.

Want to **Learn Markdown**? Check out [The Complete GitHub Markdown Cheat Sheet](https://github.com/BeyondCodeBootcamp/beyondcodebootcamp/blob/main/001-Markdown-Cheat-Sheet.md).

## Edit Post

Manage your existing posts directly on GitHub. \
Don't worry, `.GitInfo.lastmod` will pull the new "updated at" date from `git`!

> [/content/blog/][content-dir]

Just click edit, then edit and commit!

# Manual Builds

It's always nice to know that when the 💩 hits the fan, you can still get 💩
done all on your own.

1. Edit `config.yaml` to taste... \
   or `bash ./scripts/ga-template.sh`.
2. Install `hugo` and `node` via Webi:
   ```bash
   curl -sS https://webinstall.dev/hugo@v0.86 | bash
   curl -sS https://webinstall.dev/node@v16 | bash
   # or
   # bash ./scripts/install-deps.sh
   ```
3. Clone and setup repo
   ```bash
   git clone git@github.com:devPalacio/blog
   pushd ./blog
   git submodule init
   git submodule update
   hugo
   # or
   # bash ./scripts/build.sh
   ```
4. Inspect the build
   ```bash
   ls ./public
   ```
5. Deploy to GitHub pages
   ```bash
   git checkout gh-pages
   rsync -avhP public/ ./
   rm -rf public/
   git add ./
   git commit -m "deploy: latest build"
   git push
   # or
   # bash ./scripts/deploy.sh
   ```

**Something else wrong?**

Open an issue on <https://github.com/BeyondCodeBootcamp/bliss-template>.
