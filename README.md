# Artist Portfolio Website

A responsive portfolio website for a painter to showcase artwork, share their creative background, and receive inquiries about artwork commissions, exhibitions, and event bookings.

## Project Objectives

- Present the artist's work in a visually engaging way.
- Build a professional online presence.
- Help potential customers explore available artwork.
- Make it easy to request commissions or invite the artist to events.

## Key Features

- Homepage featuring selected artwork.
- Artwork gallery or portfolio.
- Artist biography and creative journey.
- Artwork details and availability, where provided.
- Commission inquiry form.
- Events and exhibitions section.
- Event invitation or booking inquiry form.
- Contact information and social links.

## Technology Stack

- **Frontend:** React.js, TypeScript
- **Backend:** Python, FastAPI
- **Database:** Supabase PostgreSQL
- **Storage:** Supabase Storage for artwork images, if required
- **Authentication:** Supabase Auth, if protected management features are needed
- **Containerization:** Docker and Docker Compose

## Architecture

React handles the user interface and artwork presentation. FastAPI supports custom APIs and inquiry processing where required. Supabase provides database and optional storage services. Docker provides a consistent development environment.

## Getting Started

### Prerequisites

- Node.js and npm
- Python 3
- Docker and Docker Compose
- A Supabase project

### Environment Configuration

Create environment files based on `.env.example`.

Frontend variables:

- `VITE_SUPABASE_URL`
- `VITE_SUPABASE_ANON_KEY`

Backend variables, where needed:

- `SUPABASE_URL`
- `SUPABASE_SERVICE_ROLE_KEY` — server-side only, if elevated access is required.

Do not commit credentials or expose privileged keys in frontend code.

### Development

Install frontend dependencies:

```bash
cd frontend
npm install
npm run dev
```

Configure backend dependencies and the FastAPI application entry point before starting the API.

Run the containerized application once Docker configuration is available:

```bash
docker compose up --build
```

## Initial Scope

The first release focuses on artwork presentation, artist information, and event or commission inquiries. Ticket sales, payment collection, calendar synchronization, and automated booking management are excluded unless separately approved.

## Quality Assurance

Test gallery responsiveness, navigation, inquiry form validation, links, and mobile layouts.

## Project Status

In development.

## License

To be determined by the project owner.
