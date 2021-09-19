#  Reading 33:NextJs Dynamic Routes

## How to statically generate pages with dynamic routes using getStaticPaths

Update the following files:

    public/images/profile.jpg with your photo (Recommended: 400px width/height).
    const name = '[Your Name]' in components/layout.js with your name.
    <p>[Your Self Introduction]</p> in pages/index.js with your self introduction.

## How to Statically Generate Pages with Dynamic Routes

    In our case, we want to create dynamic routes for blog posts:

    We want each post to have the path /posts/<id>, where <id> is the name of the markdown file under the top-level posts directory.
    Since we have ssg-ssr.md and pre-rendering.md, we’d like the paths to be /posts/ssg-ssr and /posts/pre-rendering.

## Deploying a Nex.tjs app

By using Vercel:
Develop, Preview, Ship

    We’ve just gone through the workflow we call DPS: Develop, Preview, and Ship.

    Develop: We’ve written code in Next.js and used the Next.js development server running to take advantage of its hot reloading feature.
    Preview: We’ve pushed changes to a branch on GitHub, and Vercel created a preview deployment that’s available via a URL. We can share this preview URL with others for feedback. In addition to doing code reviews, you can do deployment previews.
    Ship: We’ve merged the pull request to main to ship to production.

