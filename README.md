# ReReaddit

ReReaddit is a full-stack social discussion app built with Next.js, TypeScript, React, and PostgreSQL to provide a performant, scalable, and responsive user experience. 

## Table of Contents

- [ReReaddit](#rereaddit)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Tech Stack](#tech-stack)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Running locally](#running-locally)

---

## Features
- Create, search, and join communities of any interest
- Create, comment, upvote, and downvote posts
- User authentication and profile management  
- Media upload: users can upload images (or other media) to posts  
- Pagination for posts and comments to support efficient browsing  
- Caching of popular posts using Redis for fast retrieval  
- Responsive UI built with React + Tailwind CSS
- RESTful API architecture for communication between frontend/backend  

---

## Tech Stack

- **Frontend:** Next.js, React, TypeScript, and Tailwind CSS 
- **Backend:** Next.js routes with TypeScript  
- **Database:** PostgreSQL (Supabase), Redis (Upstash)  
- **ORM**: Prisma
- **Storage:** AWS S3 (for image / media storage)  

---

## Getting Started

### Prerequisites

Make sure you have the following installed on your local machine:

- Node.js (LTS)  
- npm or Yarn    
- AWS S3 credentials (for media uploads)  

---

### Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/rsarker1/ReReaddit.git  
   cd ReReaddit  
2. **Install the dependencies**  
    ```bash
    npm install
    # or
    yarn install
3. **Environment Variables**
    Create a ```.env``` file at the root of your project and configure the following:
    ```
    # Database
    DATABASE_URL=
    DIRECT_URL=

    NEXTAUTH_URL="http://localhost:3000"
    NEXTAUTH_SECRET=

    GOOGLE_CLIENT_ID=
    GOOGLE_CLIENT_SECRET=

    AWS_ACCESS_KEY_ID=
    AWS_SECRET_ACCESS_KEY=
    AWS_S3_BUCKET_NAME=
    AWS_REGION=

    REDIS_URL=
    REDIS_SECRET=
### Running locally
    ```bash
    # Start development server
    npm run dev  
    # or  
    yarn dev
