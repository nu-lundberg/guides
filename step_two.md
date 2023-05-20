layout: page
title: "TESTAR"
permalink: /step_two

Yes, you can easily render Markdown on GitHub Pages.

GitHub Pages is a static site hosting service that takes HTML, CSS, and JavaScript files directly from a repository on GitHub, optionally processes them through a build process, and publishes a website. 

Since GitHub Pages integrates with Jekyll, a static site generator, it inherently supports Markdown. Here are the steps:

1. **Create a new GitHub repository:** Sign in to GitHub and click the "+" icon at the top-right to create a new repository. Select "Repository" and provide a name. Let's assume the repository name is "my-project". 

2. **Clone the repository:** Use the following command on your terminal:
   
    ```bash
    git clone https://github.com/yourusername/my-project.git
    ```
   
3. **Create a new branch named "gh-pages":** This will be used to host your site.

    ```bash
    cd my-project
    git checkout -b gh-pages
    ```

4. **Add an index.md file:** Create an `index.md` file, and add some markdown to it. An example of what could be in the file:

    ```markdown
    # Hello World
    I'm hosted with GitHub Pages.
    ```

5. **Commit and push your changes:** Commit the changes and push them to GitHub. 

    ```bash
    git add .
    git commit -m "Initial commit"
    git push origin gh-pages
    ```

6. **Enable GitHub Pages:** Go back to your repository on GitHub, then to the "Settings" tab. Scroll down to the "GitHub Pages" section. Select "gh-pages branch" as the source. Save your changes.

7. **View your site:** You can now view your site at the following URL: `https://<username>.github.io/<repo-name>/`

The Markdown files that you add to your repository will automatically be converted to HTML. You can create more `.md` files and link between them to create a fully functional website. Also, Jekyll supports a layout system, themes, and much more, so you can customize your site as needed.