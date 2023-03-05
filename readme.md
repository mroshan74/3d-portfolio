# Portfolio 
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Portfolio using React, tailwind and threejs-fiber

## Features

- Use models in React
- Framer motion animation for elements
- Build using tailwind css

## Resources
- [Github Code](https://github.com/adrianhajdin/project_3D_developer_portfolio)
- [Assets, Components and Public folders](https://drive.google.com/drive/folders/1KVU8iaH0E_JFtShNiR3BgCSA3pawXY4Z)
- [Youtube](https://www.youtube.com/watch?v=0fYi8SGA20k)

## Installation
Install the dependencies and devDependencies and start the server.

```sh
npm create vite@latest
npm install --legacy-peer-deps -D tailwindcss postcss autoprefixer 
npx tailwindcss init -p
npm install --legacy-peer-deps three @react-three/fiber @react-three/drei maath react-tilt react-vertical-timeline-component @emailjs/browser framer-motion react-router-dom
```

For production environments...

```sh
```

## Plugins

Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| EmailJS | [https://www.emailjs.com/][PlDb] |

## Development

```sh
npm run dev
```

#### Building for source

For production release:

```sh
vite build
```

## Docker

By default, the Docker will expose port 3000, so change this within the
Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd 3d-portfolio
docker build -t <youruser>/3d-portfolio:${package.json.version} .
```

This will create the 3d-portfolio image and pull in the necessary dependencies.
Be sure to swap out `${package.json.version}` with the actual
version of 3d-portfolio.

Once done, run the Docker image and map the port to whatever you wish on
your host. In this example, we simply map port 8000 of the host to
port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --name=3d-portfolio <youruser>/3d-portfolio:${package.json.version}
```
Verify the deployment by navigating to your server address in
your preferred browser.

```sh
localhost:3000
```

## License

MIT

**Free Software, Hell Yeah!**