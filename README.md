# pi's patches

This fork adds support for directly using GitHub source-only releases (e.g. only the default zip-ball you get when making a new release via the GitHub UI) by recompressing them on the fly into a valid package format (remove the GitHub-added root folder) and hosting them directly on the listings page. You can specify a source-style package hosted on this listing with the `source:user/repo` syntax in the `githubRepos` section of your `sources.json`, e.g.:
```
"githubRepos": [
  "source:pimaker/animator-as-visual"
]
```

Also includes @anatawa12's fixes from https://github.com/vrchat-community/package-list-action/pull/10.

# 🤖 VPM Package Automation

This repo hosts a [Nuke](https://nuke.build/) project to help build, release and host [VPM packages](https://vcc.docs.vrchat.com/vpm/packages).

Check out the [VPM Package Template repo](https://github.com/vrchat-community/template-package) for info on how to use it.

---
For developers working on the actual automation code contained herein, you can test things locally by checking out the above template-package repo into a sibling folder of this one. If that structure doesn't work for you, check it out wherever you want and override the `LocalTestPackagesPath` parameter.