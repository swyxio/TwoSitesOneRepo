This is a demonstration of how to deploy multiple sites from one repo.

no netlify.toml is being used. instead i just push to github and use the netlify UI to set the build settings for each site.

Here's my settings for Site 1:

**Build command**: `cd site1 && npm install && npm run build`

**Publish directory**: `site1/dist`

and Here's my settings for Site 2:

**Build command**: `cd site2 && npm install && npm run build`

**Publish directory**: `site2/dist`

That's it! both build whenever someone commits to master on the repo. Not exactly fine grained control, but it works enough for most monorepo projects.

---

To see the deployed sites:

- https://twositesonerepo-site1.netlify.com/
- https://twositesonerepo-site2.netlify.com/
