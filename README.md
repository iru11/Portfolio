Irfan Nayeem — Portfolio Site

This is a one-page website about Irfan, made in a dark "cybersecurity" style. It's built with plain HTML, CSS, and JavaScript — nothing extra to install. You can send the link to people instead of a resume or LinkedIn profile.

Files in this folder
index.html                 the whole website (all the code is in this one file)
Irfan_Nayeem_Resume.pdf    the resume file the "Download Résumé" buttons open
README.md                  this file
1. Two things to fix before you publish
GitHub link. Open index.html, find the text iru11 (it's in the Contact part of the page), and change it to your real GitHub link, like https://github.com/iru11.
Link preview address. Near the top of index.html, find this line: <meta property="og:url" content="https://irfannayeem-cyber.github.io/">. Change the address to your final website link once you know it (step 3 below explains how to get it). This makes link previews in apps like WhatsApp, Slack, or email show the correct link.

A couple of optional extras:

Right now there's no phone number in the Contact section, so bots can't grab it. You can add one if you want recruiters to call you directly.
The 4 project boxes don't link to anything yet. Once those project repos are public, you can add real links to them.
2. Put the site online with GitHub Pages

Option A — using GitHub's website (no coding tools needed):

Go to github.com/new and make a new repository. Make sure it's set to public. Name it one of these ways:
<your-username>.github.io → your site's link will be just that address, or
any other name, like portfolio → your site's link will be https://<your-username>.github.io/portfolio/
On the new repository page, click "uploading an existing file", then drag in index.html and Irfan_Nayeem_Resume.pdf. Save (commit) the changes.
In the repository, go to Settings → Pages.
Under Build and deployment → Source, pick Deploy from a branch.
Under Branch, choose main and folder / (root), then click Save.
Wait a minute or two, then refresh that Pages settings page. Your live website link will show up at the top.

Option B — using git commands:

bash
cd portfolio-site
git init
git add index.html Irfan_Nayeem_Resume.pdf README.md
git commit -m "Initial portfolio site"
git branch -M main
git remote add origin https://github.com/iru11/portfolio.git
git push -u origin main

Then turn on Pages the same way as steps 3–6 above.

3. Using your own domain name (optional)

If you buy your own domain name later, add a file called CNAME to the repository with just the domain name written inside it. Then set up your domain's DNS records to point to GitHub Pages. GitHub has a guide for this: GitHub's custom domain docs.

4. Changing the content later

Everything on the site — the text, links, and colors — is inside index.html. It's split into clearly named sections (Hero, About, Skills, Experience, Projects, Certifications, Education, Contact), so you can use Ctrl+F (or Cmd+F on Mac) to find what you need. The colors are all set in one place near the top of the file, inside :root { ... }, if you want to change the look.

To change the resume file, just replace Irfan_Nayeem_Resume.pdf with your new file, keeping the same name. If you give it a different name, you'll also need to update the two places in index.html that say href="Irfan_Nayeem_Resume.pdf".
