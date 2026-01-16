# Modeling and Fabrication Techniques Class Portfolio

This is a MkDocs Material static website template for documenting a 9-day Modeling and Fabrication Techniques class. The site includes a home page with student information, portfolio, skills assessment, and course reflections, plus daily activity pages for each day of the class.

## Features

- 🎨 Beautiful Material Design theme
- 📱 Fully responsive
- 🔍 Built-in search functionality
- 🌓 Dark/Light mode toggle
- 📅 Auto-generated revision dates
- 🚀 Automatic GitHub Pages deployment

## Site Structure

- **Home Page** (`docs/index.md`): Student story, portfolio, skills level, and course view
- **Daily Activities** (`docs/daily-activities/`): 9 days of activity documentation
  - Day 1: Introduction and Fundamentals
  - Day 2-3: 3D Modeling Basics
  - Day 4-5: Material Selection and Preparation
  - Day 6-7: Advanced Fabrication Techniques
  - Day 8: Finishing and Post-Processing
  - Day 9: Final Project and Course Reflection

## Setup

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)

### Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/mkdocs_sample.git
cd mkdocs_sample
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Serve the site locally:
```bash
mkdocs serve
```

The site will be available at `http://127.0.0.1:8000`

## Configuration

### Update Site Information

Edit `mkdocs.yml` to customize:
- Site name and description
- Author name
- Repository URL
- Theme colors and features

### Customize Home Page

Edit `docs/index.md` to add:
- Your personal story
- Portfolio projects
- Skills assessment
- Course reflections

### Document Daily Activities

Edit the files in `docs/daily-activities/` to document:
- Activities completed each day
- Process documentation
- Challenges and solutions
- Key learnings
- Reflections

## Deployment to GitHub Pages

### Automatic Deployment

This repository includes a GitHub Actions workflow (`.github/workflows/ci.yml`) that automatically builds and deploys the site to GitHub Pages when you push to the `main` or `master` branch.

### Setup Steps

1. Push this repository to GitHub
2. Go to your repository settings
3. Navigate to **Pages** under **Settings**
4. Under **Source**, select **GitHub Actions**
5. The site will automatically deploy on the next push to `main` or `master`

### Manual Deployment

If you prefer to deploy manually:

```bash
mkdocs gh-deploy
```

## Customization

### Adding Images

1. Create an `images` directory in `docs/`:
```bash
mkdir docs/images
```

2. Add your images to this directory
3. Reference them in markdown files:
```markdown
![Alt text](images/your-image.jpg)
```

### Changing Theme Colors

Edit `mkdocs.yml` and modify the `palette` section:

```yaml
palette:
  - scheme: default
    primary: indigo  # Change to your preferred color
    accent: indigo   # Change to your preferred color
```

Available colors: red, pink, purple, deep-purple, indigo, blue, light-blue, cyan, teal, green, light-green, lime, yellow, amber, orange, deep-orange, brown, grey, blue-grey

### Adding New Pages

1. Create a new markdown file in `docs/`
2. Add it to the navigation in `mkdocs.yml`:

```yaml
nav:
  - Home: index.md
  - New Page: new-page.md
```

## Project Structure

```
mkdocs_sample/
├── .github/
│   └── workflows/
│       └── ci.yml              # GitHub Actions workflow
├── docs/
│   ├── daily-activities/
│   │   ├── day1.md
│   │   ├── day2.md
│   │   ├── ... (day3-9)
│   └── index.md                # Home page
├── mkdocs.yml                   # MkDocs configuration
├── requirements.txt             # Python dependencies
└── README.md                    # This file
```

## Development

### Build the Site

```bash
mkdocs build
```

This creates a `site/` directory with the static HTML files.

### Preview Changes

```bash
mkdocs serve
```

This starts a local development server that automatically reloads when you make changes.

## Troubleshooting

### Build Errors

If you encounter build errors:
1. Ensure all dependencies are installed: `pip install -r requirements.txt`
2. Check that all markdown files are valid
3. Verify image paths are correct

### GitHub Pages Not Updating

1. Check the Actions tab in your GitHub repository for workflow status
2. Ensure GitHub Pages is set to use GitHub Actions as the source
3. Verify the workflow file is in `.github/workflows/ci.yml`

## License

This template is provided as-is for educational purposes. Feel free to modify and use it for your own projects.

## Contributing

Feel free to fork this repository and customize it for your own use. If you make improvements that could benefit others, pull requests are welcome!

## Support

For issues or questions:
- MkDocs Documentation: https://www.mkdocs.org/
- Material for MkDocs: https://squidfunk.github.io/mkdocs-material/

---

**Happy documenting! 📚✨**
