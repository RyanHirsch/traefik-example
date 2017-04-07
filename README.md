# traefik-example

Before starting you need to ensure you touch `acme.json` at the root for persisting Let's Encrypt certificates.

Additional ad-hoc containers can be routeable by starting them with the correct labels.

`
docker run -d -l traefik.frontend.entryPoints=https,http -l traefik.frontend.rule=Host:dev.hirsch.io ryanhirsch/express-hello
`
