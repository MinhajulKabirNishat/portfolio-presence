# portfolio-presence
Instead of just telling people you can code, build a website to show them.
# Digital Business Card | Professional Portfolio


Instead of a traditional static resume, this "Digital Business Card" serves as a live demonstration of frontend capabilities.

## The Vision
The goal of this project is to create a high-performance, single-page application (SPA) that provides a "at-a-glance" view of my identity as a coder. It is built with a focus on clean UI, smooth transitions, and modular code.

## Tech Stack
This project is built using:

* **Framework:** [Vue.js 3](https://vuejs.org/) (Composition API)
* **Build Tool:** [Vite](https://vitejs.dev/)
* **Routing:** [Vue Router](https://router.vuejs.org/)
* **Styling:** Scoped CSS3 with custom transitions
* **Deployment:** GitHub Pages (Planned)

##  Key Features
* **Interactive Navigation:** Seamless page transitions using Vue Router without browser refreshing.
* **Reusable Components:** A dynamic `ProjectCard` system that uses Vue **Props** to display various repositories.
* **Responsive Design:** Fully optimized for mobile, tablet, and desktop screens.
* **Direct GitHub Integration:** One-click access to my source code and professional profile.

## Project Structure
```text
src/
├── assets/      # Images and global styles
├── components/  # Reusable UI parts (e.g., ProjectCard.vue)
├── views/       # Main pages (Home, Projects)
└── router/      # Navigation logic
