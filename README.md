This repository contains the source code for a podcast website built using modern web technologies. The website allows users to explore various podcasts, view podcaster profiles, and listen to episodes directly on the platform.

## Features
# User Authentication: 
Implemented using Clerk for seamless sign-in and user management.
# Podcaster Profiles: 
Users can view detailed profiles of podcasters, including their podcasts and episodes.
# Podcast Carousel: 
Showcases top podcasters and their podcasts in an interactive carousel format.
# Audio Playback: 
Integrated audio player for streaming podcast episodes directly on the site.

## Technologies Used
**Frontend:**：Built with Next.js and React.  
**Styling**: Styled using Tailwind CSS for utility-first CSS.  
**Authentication**: Managed with Clerk for user authentication and profile management.  
**Data Fetching**: Utilized Convex for real-time data queries and mutations.  
**Carousel**: Implemented using Embla Carousel for a smooth and responsive carousel experience.  

Getting Started

To get a local copy of the project up and running, follow these steps:

Clone the repository:

```
git clone https://github.com/warrenwu123/podcast-website.git
```

Navigate to the project directory:
```
cd podcast-website
```
Install dependencies:
```
npm install
```

Set up environment variables:
Create a .env.local file in the root directory and add the necessary environment variables as shown below.

```
# convex
CONVEX_DEPLOYMENT=yourconvexdeployment # this will be generated when you first run convex dev

NEXT_PUBLIC_CONVEX_URL=yourconvexpublicurl # this will be generated when you first run convex dev

# clerk

# the following codes will be found in your clerk account
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=yourpublickey
CLERK_SECRET_KEY=yoursecretkey

CLERK_WEBHOOK_SECRET=yourwebhooksecret

NEXT_PUBLIC_CLERK_SIGN_IN_URL='/sign-in'
NEXT_PUBLIC_CLERK_SIGN_UP_URL='/sign-up'

OPENAI_API_KEY=youropenaiapikey # this will be found at your own openai setting interface

```

Run the development server:
```
npm run dev
```
Open your browser and navigate to http://localhost:3000 to view the website.
