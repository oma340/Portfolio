INNOCENT OMALE PORTFOLIO - HOSTING GUIDE

FOLDER CONTENTS
  index.html            the website
  admin/                the hidden admin page (yoursite.com/admin)
  content/              your projects and settings (the admin edits these)
  images/uploads/       your uploaded images land here

STEP 1: PUT THE FILES ON GITHUB
  1. Create a free account at github.com.
  2. Create a new repository (name it e.g. "portfolio"). Choose Public or Private.
  3. Upload everything in this folder to it, keeping the same folders.

STEP 2: CONNECT NETLIFY
  1. Create a free account at netlify.com (sign in with GitHub).
  2. Add new site > Import an existing project > choose your GitHub repo.
  3. Leave build settings empty. Publish directory: leave blank or "/".
  4. Deploy. Rename the site under Site configuration > Change site name.

STEP 3: POINT THE ADMIN AT YOUR REPO
  Open admin/config.yml on GitHub and change
    repo: YOUR-GITHUB-USERNAME/YOUR-REPO-NAME
  to your real username and repo name. Save (commit).

STEP 4: LOG IN TO THE ADMIN
  Go to yoursite.netlify.app/admin and sign in with GitHub.
  If the login asks for a token, create a GitHub personal access token that can
  edit this one repository, and paste it in. Keep it private.

USING IT
  Projects, Contact, Portrait and Logo each have a form. Save, and Netlify
  rebuilds the site by itself in about a minute.
  Tip: export images at about 1600 px wide before uploading so the site stays fast.
