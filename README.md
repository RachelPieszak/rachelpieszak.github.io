## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/RachelPieszak/rachelpieszak.github.io/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Docs on adding content to portfolio / etc

If you have a new image you want to add to the portfolio, just add it to the folder `/assets/portfolio`, and then in `/portfolio.html`, add that "type" (blogpost, landingpage, email, publication, print) by copy/pasting one of the same type, and updating all the things with your new image.

Every portfolio piece is divded into different categories: `filter-{something}` so figure out which one it is.

```html
<li data-filter=".filter-landingpage">Landing Page</li>
<li data-filter=".filter-blogpost">Blog Post</li>
<li data-filter=".filter-email">Email</li>
<!-- <li data-filter=".filter-web">Social</li> -->
<li data-filter=".filter-publication">Publication</li>
<li data-filter=".filter-print">Print</li>
```

When you know what type it is, let's say `filter-email`, go and find one on that `portfolio.html` page and copy the entire section.

#### Adding a new portfolio item 

> The only things you need to change are both the **img** and **a** tags to point to your new image, update the **h4** and **title** within the `<a>` tag. More info below.

```html
<div class="col-lg-4 col-md-6 portfolio-item filter-email">
    <div class="portfolio-wrap">
        <img src="assets/portfolio/veritone-email-1.png" class="img-fluid" alt=""> <!-- 👈 update image src -->
        <div class="portfolio-info">
        <h4>Veritone One</h4> <!-- 👈 update Name -->
        <p>Email</p>
        <div class="portfolio-links">
            <!-- 👇 a href -->
            <a href="assets/portfolio/veritone-email-1.png" data-gall="portfolioGallery" class="venobox" title="Veritone One - Email"> <!-- 👈 update title="" here -->
            <i class="bx bx-expand-alt"></i> <span>View Larger</span>
            </a>
        </div>
        </div>
    </div>
</div>
```

And that's it!

### Claude HTML files

> You can put these files in the `/claude` folder.

- If Claude gives you HTML just make a "new file" in `/claude` here in this project.
- Call the file `whatever.html` (it just needs the `.html` ending).  
- Copy/paste all the HTML in the new file.
- To preview the HTML file **right click** on the file (in the left sidebar), and click "Reveal in Finder".
- Now double click the file to open it in Chrome.
- In Chrome, click the `Camera` 📷 icon in the Extensions toolbar up top (to take a screenshot of the whole page)
- Now `Download` the image, and put it in this project under `/assets/portfolio/name-it-whatever.png` (and remember the name).

Now that you have the file/image here in this project, you can go to `portfolio.html` file (in the sidebar), and add it!

Look above to see how to add it to portfolio.

Buzi 💜 -M