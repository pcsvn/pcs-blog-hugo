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
