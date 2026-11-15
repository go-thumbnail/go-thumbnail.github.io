# go-thumbnail.github.io

Source for the **go-thumbnail** organization landing page at
<https://go-thumbnail.github.io/>, built with [Hugo](https://gohugo.io/)
(self-contained layouts, no theme). Pushes to `main` build and deploy to
GitHub Pages via `.github/workflows/hugo.yml`.

```sh
hugo server   # local preview
```

BSD-3-Clause.

## The design is not here

It comes from the shared Hugo module
[`go-fleettools/landingkit`](https://github.com/go-fleettools/landingkit),
pinned in `go.mod` (Renovate bumps it); `kit.go` keeps `go mod tidy` from
deleting that requirement. `[params.brand]` in `hugo.toml` is read from the logo by
`landingkit brand`. A file under `layouts/partials/` with the name of one of the
kit's would silently override it.
