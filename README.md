## TEMU Website sources

Website is generated from static markdown pages under ```./content``` using [hugo](https://gohugo.io).

The website is hosted by github pages from a separate [repository](https://github.com/temu-ltky/temu-ltky.github.io).

See [Hugo's documentation](https://gohugo.io/getting-started/) and github pages' [deploy guide](https://gohugo.io/hosting-and-deployment/hosting-on-github/#host-github-user-or-organization-pages) for more information.



To serve your site locally:

```bash
docker run --rm -it -v $PWD:/src -p 1313:1313 -u hugo jguyomard/hugo-builder hugo server -w --bind=0.0.0.0
```

Then open [`http://localhost:1313/`](http://localhost:1313/) in your browser.

To build your site:

```bash
docker run --rm -it -v $PWD:/src -u hugo jguyomard/hugo-builder hugo
```


More information can be found in [docker image's documentation](https://github.com/jguyomard/docker-hugo)
