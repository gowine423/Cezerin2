

# Cezerin is React and Node.js based eCommerce platform. React Shopping Cart.

Cezerin - Ecommerce Progressive Web Apps. Complete Solution.

## Cezerin Platform:

1. Cezerin API - Backend.
2. Cezerin Store - Frontend.
3. Cezerin Admin - Dashboard.
4. Cezerin Client - JavaScript client for Cezerin REST API.

## Built with:

- NodeJS
- ReactJs
- Redux
- ExpressJs
- Babel
- WebPack
- MongoDB


## Store

Single-Page Application with React server-side rendering.

SEO Friendly. Google Analytics eCommerce Tracking included.

[Online Demo Store - Plusha Theme](https://plusha.demo.chost.ansiglobal.com)

[![Cezerin Store Plusha Theme](https://chost.ansiglobal.com/img/cezerin-plusha-theme.png)](https://plusha.demo.chost.ansiglobal.com)

[Online Demo Store - Default Theme](https://demo.chost.ansiglobal.com)

[![Cezerin Store Default Theme](https://chost.ansiglobal.com/img/cezerin-default-theme.png)](https://demo.chost.ansiglobal.com)
[![Cezerin Store Default Theme](https://chost.ansiglobal.com/img/cezerin-mobile-order-summary.png)](https://demo.chost.ansiglobal.com)

## Dashboard

Client-side dashboard use JSON Web Token (JWT) to access REST API.

[Online Demo Dashboard](https://demo.chost.ansiglobal.com/admin)

![Cezerin Dashboard](https://chost.ansiglobal.com/img/cezerin-dashboard-products.png)

## Docs

- Getting Started

  - [Overview](./docs/overview.md)
  - [Online Demo](./docs/online-demo.md)
  - [Application Structure](./docs/application-structure.md)
  - [API Client](https://github.com/cezerin2/cezerin2-client)
  - [API Reference](https://github.com/Cezerin2/Cezerin2/tree/main/docs/api)

- Installation Guides

  - [Prerequisites](./docs/prerequisites.md)
  - [Setup Database](./docs/setup-database.md)
  - [Using source code](./docs/using-source-code.md)
  - [Using docker](./docs/using-docker.md)

- Deploy on Web

  - [Hosting](./docs/deploy-on-web-hosting.md)
  - [Create droplet](./docs/deploy-on-web-droplet.md)
  - [Setup domain](./docs/deploy-on-web-domain.md)
  - [Install NGinx Web Server + MERN Stack](./docs/deploy-on-web-mern.md)
  - [Run MongoDB](./docs/deploy-on-web-mongodb.md)
  - [Run Cezerin](./docs/deploy-on-web-cezerin.md)
  - [Run NGinx](./docs/deploy-on-web-nginx.md)
  - [Cezerin configs changes](./docs/deploy-on-web-cezerin-configs.md)
  - [Final checks](./docs/deploy-on-web-final-checks.md)
  - [Setup Let's Encrypt SSL Certificate](./docs/deploy-on-web-lets-encrypt.md)
  - [Turn off Developer Mode](./docs/deploy-on-web-production-mode.md)

- API

  - [API Reference](./docs/api)

- Help
  - [FAQ](./docs/faq.md)
  - [HowTos](./docs/howtos.md)
  - [Help and Support](./docs/help-and-support.md)

### Requirements

- [Node.js - LTS](https://nodejs.org/en)
- [Yarn](https://yarnpkg.com/getting-started/install)
- [MongoDB](https://docs.mongodb.com/manual/installation)


### Quick Start

##### On your local machine

If you have installed above requirements,

1. [Download code](https://github.com/gowine423/Cezerin2/archive/refs/heads/main.zip)
2. Extract code, update config at config folder as you need and run setup.sh on the folder
3. To setup required mongodb collections you will need to run `yarn setup` from command line in the folder

##### On Digitalocean Droplet

1. Start a basic ubuntu server
2. Run `curl -o- https://raw.githubusercontent.com/Cezerin2/Cezerin2/main/scripts/droplet.sh | bash` in the command line
3. You can update config from config folder as required and restart server by running `yarn build` and `pm2 start process.json`

## Application Structure

```
.
├── config                   # Project and build configurations
├── dist                     # Distribution folder
├── locales                  # Text files
├── logs                     # Log files
├── public                   # Static public assets and uploads
│   ├── admin                # Dashboard index.html
│   ├── admin-assets         # Dashboard assets
│   └── content              # Store root folder
|
├── scripts                  # Shell scripts for theme install/export
├── src                      # Application source code
│   ├── admin                # Dashboard application
│   │   └── client           # Client side code
│   ├── api                  # REST API
│   │   └── server           # Server side code
│   └── store                # Store application
│       ├── client             # Client side code
│       ├── server             # Server side code
│       └── shared             # Universal code
|
├── theme                    # Theme as a local package
└── process.json             # pm2 process file
```

## Yarn Scripts

| `yarn <script>` | Description                                                 |
| --------------- | ----------------------------------------------------------- |
| `setup`         | Run Cezerin mongodb setup.                                  |
| `theme:export`  | Zip current theme to /public/<file>.zip                     |
| `theme:install` | Install theme from /public/<file>.zip                       |
| `build:store`   | Builds the store for production to the dist folder.         |
| `build:admin`   | Builds the admin for production to the public/admin folder. |
| `build`         | Build everything for production.                            |
| `start:store`   | Runs the store in production mode.                          |
| `start:server`  | Runs the server in production mode.                         |
| `start`         | Run everything in production mode.                          |
| `watch:store`   | Runs the store in development mode.                         |
| `watch:admin`   | Runs the admin in development mode.                         |
| `watch:server`  | Runs the server in development mode.                        |
| `watch`         | Run everything in development mode.                         |
| `lint`          | Check project with eslint.                                  |

## Financial contributions

We also welcome financial contributions in full transparency on our [open collective](https://opencollective.com/cezerin2).
Anyone can file an expense. If the expense makes sense for the development of the community, it will be "merged" in the ledger of our open collective by the core contributors and the person who filed the expense will be reimbursed.

## Credits

### Contributors

Thank you to all the people who have already contributed to cezerin2!

<img src="https://github.com/ekarailiev.png" alt="Emil K." height="36" style="border-radius: 100%" />
<a href="https://github.com/gowine423/cezerin2/graphs/contributors"><img src="https://opencollective.com/cezerin2/contributors.svg?width=890" /></a>

## Contributing

If you can, please contribute by reporting issues, discussing ideas, or submitting pull requests with patches and new features. We do our best to respond to all issues and pull requests within a day or two, and make patch releases to npm regularly.

## Licence

This software is provided free of charge and without restriction under the MIT License
