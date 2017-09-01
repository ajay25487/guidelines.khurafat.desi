# New Project Setup

## Git

Create a repository on the Khurafat organization on GitHub.

## Server

1. Provision a new server on Forge. Use a kebab-cased version of the domain name for the droplet (example: `guidelines-khurafat-desi`)
1. Create a new site with root `/public`
1. Ensure the name of the database makes sense
1. Start a queue worker: `default`
1. Update the relevant `.env` variables. Don't forget to add the necessary service API keys later.
1. Enable backups in Ottomatik for the project

## Services

Unless specified otherwise, use the website's domain name as its identifier (API key name, property name, etc.)

1. Create a new **Sendgrid** API key
1. Create a new **Google Analytics** property
1. Create a new **Google Tag Manager** container
    - Create a constant containing the Universal Analytics ID
    - Set up a tag for Google Analytics pageviews
1. Set up **Bugsnag** for Laravel
1. Set up **Bugsnag** for JavaScript
