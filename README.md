# Personal Portfolio Website

A modern, responsive portfolio website built with Vue.js and TypeScript. Features a clean design with warm accent colors and showcases projects, games, and contact information.

## 🚀 Quick Start

### Prerequisites
- Node.js (v12 or higher)
- npm (comes with Node.js)
- Git

### Fork and Clone
1. Fork this repository by clicking the 'Fork' button at the top right of this page
2. Clone your forked repository:
```bash
git clone https://github.com/YOUR_USERNAME/hurshh.github.io.git
cd hurshh.github.io
```

### Install Dependencies
Install all required dependencies:
```bash
npm install
```

### Run Development Server
Start the development server:
```bash
npm run serve
```
The site will be available at `http://localhost:8080`

## 🛠️ Development

### Project Structure
```
src/
├── components/     # Vue components
├── views/         # Page components
├── css/           # Styles and variables
├── data/          # Project data files
├── router/        # Vue router configuration
└── App.vue        # Root component
```

### Key Features
- Vue.js with TypeScript support
- Responsive design
- Project showcase sections
- Contact form
- Game projects section
- Clean, modern UI with warm accent colors

### Available Scripts
- `npm run serve` - Start development server
- `npm run build` - Create production build
- `npm run lint` - Lint and fix files

## 📝 Customization

### Updating Content
1. Project data is stored in `src/data/` directory:
   - `GameProjectsData.ts` - Game projects
   - `OtherProjectsData.ts` - Other projects
   - `ProjectData.ts` - Project interface definitions

2. Update images in `public/img/` directory

### Styling
- Main color variables are in `src/css/variables.less`
- Project-specific styles in `src/css/projects.less`
- Component-specific styles in their respective `.vue` files

## 🚀 Deployment
This portfolio is configured for GitHub Pages deployment:

1. Update the repository name to `YOUR_USERNAME.github.io`
2. Enable GitHub Pages in repository settings
3. Build and deploy:
```bash
npm run build
git add docs
git commit -m "deploy: update build"
git push
```

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'feat: add amazing feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Contact
If you have any questions or suggestions, feel free to reach out through the contact form on the website.
