Repository for documentation of eol projects

# Docs EOL

## Development

In the project directory you have to run:

### `docker-compose up -d docs-m4s`

Runs the app in the development mode. Open http://localhost:3005 to view it in the browser.

## Build production

In the project directory you have to run:

### `docker-compose exec docs-m4s bash`

### `npm run build`

The build folder will be ready to be deployed.
<br> <br>

## Working with the Docker container in development

To build the Docker container for development, run:

### `docker build --target development -t docs:dev .`

To run the Docker container in development, run:

### `docker run -p 3000:3000 docs:dev`

### Note: Remember to stop the container before proceeding to the next step.

## Working with Docker container in production

To build the Docker container for production, run:

### `docker build -t docusaurus:latest .`

To run the Docker container in production, run:

### `docker run --rm -p 3000:3000 docusaurus:latest`
