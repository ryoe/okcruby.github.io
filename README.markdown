## okcruby.github.io AKA www.okcruby.org

### Contributing

This site is powered by [Octopress](http://octopress.org/).  You should not work directly in the
`master` branch, but in the `source` branch.

To checkout this repo to begin working you only need the `source`
branch:

```
git clone git@github.com:okcruby/okcruby.github.io.git -b source okcruby.github.io
```

Then you need to setup the `_deploy` directory:

```    
mkdir _deploy
cd _deploy
git init
git remote add -t master -f origin git@github.com:okcruby/okcruby.github.io.git
```

Anytime that you want to make changes to the site you should first make
sure to pull from the master repo on Github.

```
git pull --rebase
```

Then make your changes and commit (to the source branch).  Then to deploy
you can run:

```
rake generate
rake deploy
```




See the [Octopress Blogging Basics Guide](http://octopress.org/docs/blogging/) for the basics of working with the site.

**Note**: Octopress requires a minimum Ruby version of `1.9.3-p0`.
