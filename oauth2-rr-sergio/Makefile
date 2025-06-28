# Declares phony targets to prevent conflicts with files named api, idp, web, or e2e
.PHONY: api idp web e2e

api:
	cd api && bun start

idp:
	cd idp && bun start

web:
	cd web && bun run dev

start:
	make idp & make api & make web

e2e:
	bun run --filter e2e test