# ProjectShare

A full-stack (React/Flask/Postgres) web app that allows developers to easily browse and share GitHub projects.

- uses OpenAI's ChatGPT API for text generation and DALL-E API for text-to-image generation to streamline project sharing

- implements full-stack JWT user authentication, project tagging/filtering, and a comment system.

<a href="https://projectshare-frontend-react.onrender.com/ " target="_blank">View Live Project</a>

 Note: projects can take a few seconds to show up the first time as the backend "wakes up"

[View Frontend React/Tailwind Repository](https://github.com/quentin-mckay/ProjectShare-Frontend-React)

[View Backend Flask/Postgres Repository](https://github.com/quentin-mckay/ProjectShare-Backend-Flask)

<!-- <div style="display: grid; grid-template-columns: 1fr 1fr;">
	<a href="https://github.com/quentin-mckay/ProjectShare-Frontend-React">View React Frontend</a>
	<a href="https://github.com/quentin-mckay/ProjectShare-Backend-Flask">View Flask Backend</a>
</div> -->

[![logged in](./images/projectshare_home.jpg)](https://projectshare-frontend-react.onrender.com/)

## Tech Used

**Frontend**

- React v18
- React Router v6
- React Context API (for managing global auth state)
- Axios (for data fetching)
- Framer Motion (for page transitions)
- Tailwind CSS (for all styles)

**Backend**

- Flask
- PostgreSQL
- Flask-SQLAlchemy (ORM)
- OpenAI ChatGPT API (model gpt-3.5-turbo)
- OpenAI DALL-E API (text-to-image generation)
- Cloudinary API (image storage/retrieval)

**Tools**

- Vite (build)
- Render (deployment)

## Features

**Full-Stack Authentication**

- Only users who have signed up or logged in can post new projects.

- Logged in users see Edit/Delete buttons on only their projects.

- Logged in users see a button with their name in the upper right that can be clicked to show their projects

- browser remembers logged in user

**OpenAI Integration**

- When posting a project, users can click a button to have ChatGPT auto-fill the project description using just the GitHub repository link. The first sentence of the description will be seen on the project card but the entire description is visible on the project page.

- Users can also generate a cover image for their project by prompting OpenAI's DALL-E text-to-image generator (or let ChatGPT auto-generate a prompt). Images are stored using Cloudinary, a media management platform.

**Tag System**

- Users can enter tags for their project (uses a 3rd party package called )

- These tags can then be clicked (either on the project card or project page) to show only projects which have that tag.

**User Filtering**

- Clicking on a project author's name (either on the project card or project page) will show only projects by that author.

**Comment System**

- Users can leave comments on other projects.

**Page Transitions**

- Framer Motion was used to create subtle fades between pages.

## Screenshots

![create project page](./images/projectshare_create.png)

![project page](./images/projectshare_projectpage.png)

![signup page](./images/projectshare_signup.png)

![logged in](./images/projectshare_loggedin.jpg)

