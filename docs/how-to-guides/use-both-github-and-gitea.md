# Use both GitHub and Gitea

Even though we self-host Gitea, you may still want to use GitHub as a backup and for discovery.

Add both push URLs (replace my repositories with yours):

```sh
git remote set-url --add --push origin git@git.iuliandita.com:ops/homelab
git remote set-url --add --push origin git@github.com:iuliandita/homelab
```

Now you can just run `git push` like usual and it will push to both GitHub and Gitea.
