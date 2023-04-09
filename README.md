# ProjectShare

A web app that allows developers to easily browse and share GitHub projects.

[View Live Project](https://projectshare-frontend-react.onrender.com/)

<!-- [React Frontend Repository](https://github.com/quentin-mckay/ProjectShare-Frontend-React)

[Flask Backend Repository](https://github.com/quentin-mckay/ProjectShare-Backend-Flask) -->


<div style="display: grid; grid-template-columns: 1fr 1fr;">
	<a href="https://github.com/quentin-mckay/ProjectShare-Frontend-React">View React Frontend</a>
	<a href="https://github.com/quentin-mckay/ProjectShare-Backend-Flask">View Flask Backend</a>
</div>

<hr>

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

**Build Tool**

- Vite

## Features

**Full-Stack Authentication**

Anyone can view posted projects but only users who have signed up or logged in can post new projects.

Logged in users will see Edit/Delete buttons on their projects only.

**AI Assistance**

When posting a project, users can click a button to have ChatGPT auto-fill the project description using just the GitHub repository link.

Users can also generate a cover image for their project by prompting OpenAI's DALL-E text-to-image generator (or let ChatGPT auto-generate a prompt).

**Tag Filtering**

Users can enter tags for their project. These tags can then be clicked by other users to filter on those projects which have that tag.

**User Filtering**

Clicking on a project author's name will filter projects by that author.

**Comments**

Users can leave comments on other people projects.



