To deploy your React portfolio to `<username>.github.io`, you'll need to create a new repository specifically for that purpose. Here are the steps:

1. **Create a new repository**: On GitHub, create a new repository with the name `<username>.github.io`, where `<username>` is your GitHub username. This is a special repository name that GitHub uses to serve the content as a website on `<username>.github.io`.

2. **Clone the repository**: Clone the newly created repository to your local machine using the command:

```
git clone https://github.com/<username>/<username>.github.io.git
```

3. **Copy your React build files**: After running `npm run build` (or `yarn build`) in your React project, copy the contents of the `build` folder into the cloned `<username>.github.io` repository.

4. **Commit and push changes**: Inside the `<username>.github.io` repository, commit and push the changes to GitHub:

```
git add .
git commit -m "Initial deploy"
git push origin main
```

5. **Enable GitHub Pages**: In your `<username>.github.io` repository settings on GitHub, go to the "Pages" section and ensure that the source is set to the `main` branch (or any other branch you want to use for deployment).

6. **Access your portfolio**: After a few minutes, your portfolio should be live at `https://<username>.github.io`.

From now on, whenever you want to update your portfolio, you'll need to rebuild your React app, copy the new `build` folder contents into the `<username>.github.io` repository, and commit and push the changes to GitHub.

Note that if you want to use a custom domain for your portfolio, you can configure it in the "Custom domain" section of your `<username>.github.io` repository's settings on GitHub.
