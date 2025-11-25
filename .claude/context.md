# AI Context: Groene-rust Holiday Rental Website

## Project Overview
This is a single-page static website for a holiday rental home called "Groene-rust" (Green Rust). Built with Astro for optimal performance and SEO.

## Technology Stack
- **Framework**: Astro (static site generator)
- **Language**: TypeScript/JavaScript
- **Styling**: Tailwind CSS
- **Deployment**: [To be defined]

## Project Structure
```
Groene-rust/
├── src/
│   ├── pages/
│   │   └── index.astro          # Main single-page site
│   ├── components/               # Reusable Astro components
│   ├── layouts/                  # Page layouts (if needed)
│   ├── images/                   # Optimized images (Astro will process these)
│   └── styles/                   # Global styles
├── public/                       # Static assets (favicon, etc.)
│   └── favicon.svg
└── astro.config.mjs             # Astro configuration
```

## Site Architecture
This is a **single-page website** with all content on the index page. The site should include typical holiday rental sections:
- Hero section with main image
- Property overview/description
- Amenities/features
- Photo gallery
- Location/area information
- Availability/booking information
- Contact information

## Astro Conventions to Follow

### Component Structure
- Use `.astro` files for components with static content
- Keep components in `src/components/`
- Use descriptive component names (e.g., `HeroSection.astro`, `AmenitiesList.astro`)

### Styling Approach
- Scoped styles within Astro components using `<style>` tags
- Global styles in `src/styles/`
- Follow mobile-first responsive design

### Content Management
- Content can be defined in the frontmatter of `index.astro`
- Images should be placed in `public/` folder
- Optimize images for web performance

### Performance Best Practices
- Leverage Astro's zero JavaScript by default
- Only add client-side JavaScript when necessary (use `client:*` directives)
- Optimize images (use WebP, appropriate sizes)
- Minimize CSS and keep it scoped

## Code Style Preferences
- Use TypeScript where applicable
- Semantic HTML5 elements
- Accessible markup (ARIA labels, alt text, proper heading hierarchy)
- Clean, readable code with comments for complex sections

## SEO Considerations
- Proper meta tags (title, description, Open Graph)
- Structured data for vacation rental (Schema.org)
- Semantic HTML for better crawling
- Optimized images with alt text

## Naming Conventions
- Components: PascalCase (e.g., `BookingForm.astro`)
- Files/folders: kebab-case (e.g., `hero-section.astro`)
- CSS classes: kebab-case (e.g., `hero-section`, `amenities-grid`)
- Variables: camelCase

## Development Workflow
- Run dev server: `npm run dev`
- Build for production: `npm run build`
- Preview production build: `npm run preview`

## Content Guidelines
The site should convey:
- Welcoming, relaxing atmosphere
- Clear information about the property
- Easy way to contact or book
- Professional yet warm tone
- High-quality imagery

## Notes for AI Assistants
- This is a single-page site - all content goes in `src/pages/index.astro`
- Focus on performance and SEO as this is a commercial website
- Ensure mobile responsiveness (many users will browse on phones)
- Keep the design clean and focused on the property
- Prioritize fast loading times
- When creating components, extract reusable sections from index.astro
