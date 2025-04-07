# Cloudflare Pipelines

This is the starter template for Pipelines, which let you ingest real time data streams and load into R2. This template lets you send data from a Cloudflare Worker, to a pipeline.

* Clone this repository to get started with sending data from a Worker to a pipeline.
* Review the [Pipelines developer documentation](https://developers.cloudflare.com/pipelines/) to dive deeper into how Pipelines Works

## Usage

### Create a pipeline
**Visit the [getting started guide](https://developers.cloudflare.com/pipelines/getting-started/) for Pipelines for a full guide to creating your first pipeline.**

If you already have a Cloudflare Workers paid account, get started quickly by running this command to create an R2 bucket, and create a pipeline:
```sh
npx wrangler@latest r2 bucket create pipelines-starter-bucket
npx wrangler@latest pipelines create pipeline-starter --r2-bucket pipelines-starter-bucket
```

### Deploy it
You can create a project using this template by using `npm create cloudflare@latest`:

```sh
npm create cloudflare@latest pipelines-starter -- --template "cloudflare/pipelines-starter"
```

This will automatically clone this repository, install the dependencies, and prompt you to optionally deploy:

```sh
╭ Create an application with Cloudflare Step 1 of 3
│
├ In which directory do you want to create your application?
│ dir ./pipelines-starter
│
├ What would you like to start with?
│ category Template from a GitHub repo
│
├ What's the url of git repo containing the template you'd like to use?
│ repository cloudflare/pipelines-starter
│
├ Cloning template from: cloudflare/pipelines-starter
│
├ template cloned and validated
│
├ Copying template files
│ files copied to project directory
│
├ Installing dependencies
│ installed via `npm install`
│
╰ Application created

╭ Configuring your application for Cloudflare Step 2 of 3
│
├ Installing @cloudflare/workers-types
│ installed via npm
│
├ Adding latest types to `tsconfig.json`
│ added @cloudflare/workers-types/2023-07-01
│
├ Do you want to use git for version control?
│ yes git
│
├ Initializing git repo
│ initialized git
│
├ Committing new files
│ git commit
│
╰ Application configured

╭ Deploy with Cloudflare Step 3 of 3
│
├ Do you want to deploy your application?
│ no deploy via `npm run deploy`
│
╰ Done

────────────────────────────────────────────────────────────
🎉  SUCCESS  Application created successfully!
```

The [Pipelines documentation](https://developers.cloudflare.com/pipelines/) contains examples, the API reference, and architecture guidance.

## License

Copyright 2025, Cloudflare. Apache 2.0 licensed. See the LICENSE file for details.
