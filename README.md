## Add Workflow
```Create Dev container in VS Code

{
	"name": "Debian",
	"image": "mcr.microsoft.com/devcontainers/base:bullseye",
	"features": {
		"ghcr.io/devcontainers/features/git:1": {},
		"ghcr.io/devcontainers/features/go:1": {},
		"ghcr.io/devcontainers/features/hugo:1": {
			"extended": true
		}
	},
	"postStartCommand": "hugo server"
}
```
Tree
.
├── archetypes
├── content
│   └── posts
│       ├── about.md
│       ├── image.png
│       ├── my-2nd-post.md
│       └── my-first-post.md
├── hugo.toml
├── pcsvn.github.io ### This folder is submodule !!!
│   ├── index.html
│   ├── index.xml
│   ├── page
│   ├── posts
│   │   ├── about
│   │   ├── image.png
│   │   ├── index.html
│   │   ├── index.xml
│   │   ├── my-2nd-post
│   │   ├── my-first-post
│   │   └── page
│   ├── sitemap.xml
│   ├── svg
│   └── tags
├── README.md
├── resources
└── themes
    └── LoveIt