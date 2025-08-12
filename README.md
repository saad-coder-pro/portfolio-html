## Folder Structure

```bash
├── src
│   ├── index.html
│   ├── css
│   │   ├── style.css
│   │   ├── utilities.css
│   ├── assets
│   │   ├── favicon
│   │   │   ├── android-chrome-192x192
│   │   │   ├── android-chrome-512x512
│   │   │   ├── apple-touch-icon
│   │   │   ├── favicon-16x16
│   │   │   ├── favicon-32x32
│   │   │   ├── favicon.ico
│   │   │   ├── site.webmanifest   
│   │   ├── profile-image
│   │   ├── logo
│   ├── js
│   │   ├── script.js
├── .github
│   ├── ISSUE_TEMPLATE
│   │   ├── bug.md
│   │   ├── feature.md
│   ├── Pull_request_template.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── REQUIREMENTS.md
├── package.json
└── .gitignore
```

<div align="center">
    <h1>✨ How to Customize this Template ✨</h1>
</div>
This portfolio uses modern HTML5 semantic tags like article, header, footer and more for better accessibility and improve SEO, you can read more about that on Jemima's article: <a href="https://blog.jemimaabu.com/how-to-improve-your-seo-ranking">How to improve your SEO ranking</a>.  
Also learn about metatags and how to generate them for SEO optimization <a href="https://github.com/CommunityPro/portfolio-html/blob/main//Metatags.md">here</a>.

The root page of this project is located at `/docs/index.html` This is the default page you see when you visit the site.
Want to customize this template to suit your style, here are a few things you can change: 

## 1. Logo
The logo of this template is controlled by this line in the `index.html` markup, replace the `./assets/logo.png` with your logo link or replace the current logo image without yours and rename it to `logo.png`

```html
<!-- Logo -->
<h1 id="logo">
    <a href="#"><img src="./assets/logo.png" alt="Your Logo"></a>
</h1>
```

## 2. Navigation Links
```html
<ul class="nav-menu">
   <li><a class="nav-link" href="#">PROJECTS</a></li>
   <li><a class="nav-link" href="#">CONTACT</a></li>
   <li><a class="nav-link" href="#">BlOG</a></li>
   <li><a class="nav-link btn btn-primary" href="#">RESUME <i class="fas fa-arrow-right"></i></a>
   </li>     
</ul>
```
Replace the `#` symbol with your respective link. Delete any `nav-link` that is not being used or edit the name with your own preferred link source.
- The last navigation link is the highlighted yellow button on the template. Which is styled with the `btn` & `btn-primary` classes.

## 3. Profile Image
Replace the icon or user profile with your profile image. Image can be found in the `/assets/profile-image.png`.
```html
<img class="profile-image" src="./assets/profile-image.png" alt="" />
```
You can add the image locally by replacing it with the `/assets/profile-image.png`.
Or replace the `src` link in the HTML file with your preferred image. I recommend you copy your GitHub profile image link, so the image changes anytime you update it on GitHub.

## 4. Name
Edit the name on the welcome message with your own name. This line of text can be found in the `/docs/index.html` file.
Replace `Franklin` with your own name. 
```html
<h1>Hi I'm Franklin</h1>
```

## 5. Job Title
Summarize what you do in five words and add it into the `<h2></h2>` line. Add the first two in the first `<h2>` element and add the remaining four on the next `<h2>`
```html
<h2>Building digital</h2>
<h2>products, brands, and experience.</h2>
```

## 6. Job Description
Update the job description with your information. 20 words recommended.
```html
<p>
  A Frontend Developer and Visual Designer with experience in web
  design, brand identity and product design.
</p>
```

## 7. Connect With Me
Replace the `#` on the connect with me button with a link. You can choose what link you want your visitors to go when they click this button. Social links, email address or phone number, it's completely up to you.
```html
<a href="#" class="btn btn-secondary">Connect With Me</a>
```
- Email: `<a href="mailto:user@gmail.com" class="btn btn-secondary">Connect With Me</a>`
OR
- Phone: `<a href="tel:+23400000000" class="btn btn-secondary">Connect With Me</a>`

## 8. Project
This section showcases your projects using screenshots. It has 3 columns and 2 rows by default but you can add more columns according to your use case. 
The `.project` controls the number of columns and rows of the project cards. 

```html
<div href="" class="card">
   <div class="project-info">
      <div class="project-bio">
         <h3>Project One</h3>
         <p>React, Redux, SASS</p>
      </div>

      <div class="project-link">
         <a href="#"><i class="fab fa-github"></i></a>
         <a href="#"><i class="fas fa-globe"></i></a>
      </div>
   </div>
</div>
```

To customize the cards, here are a few things you can change:
### Project Title
```html
<h3>Project One</h3>
```
This is controlled by the `<h3></h3>` element. Edit the text and add your preferred project name.

### Project Stack
This is where you display the tools/technologies used in building the project. Edit the `<p></p>` element with the specific tools or delete the line completely.
```html 
<p>React, Redux, SASS</p>
```
### Project Link
The project links are the icons on the top right of the project cards. One is the github link and the other is the live link. You can paste the respective links into the empty `href` attributes. The icons are added using an icon library called <a href="fontawesome.com/">fontawesome</a> so changing this icon is super easy.
```html
<a href="#"><i class="fab fa-github"></i></a>
<a href="#"><i class="fas fa-globe"></i></a>
```

## Project Styling
The layout of the project cards is controlled by the `.project` in the `style.css` file. By using CSS `grid-template-columns`, the cards are outlined on three columns on desktop mode, two columns on tablet mode and one column on mobile view. 

```css
.project {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-auto-rows: minmax(250px, auto);
  grid-gap: 0.9rem;
}
```

## Social Links
The footer links contain social icons that you can link to your specific social channels. By default the icons available are: `Facebook`, `Twitter`, `LinkedIn`, `GitHub`, `Hashnode` and the icons image are added locally to the assets folder, so you can add your own custom icon and link it. 

```html
<a href="mailto:communitypro47@gmail.com">communitypro47@gmail.com</a>
 <div class="social">
    <a href="#"><img src="./assets/facebook-icon.svg" alt="Facebook"></a>
    <a href="#"><img src="./assets/twitter-icon.svg" alt="Twitter"></a>
    <a href="#"><img src="./assets/linkedin-icon.svg" alt="Linkedin"></a>
    <a href="#"><img src="./assets/github-icon.svg" alt="GitHub"></a>
    <a href="#"><img src="./assets/hashnode-icon.svg" alt="Hashnode"></a>
 </div>
```

## META Tags
Use <a href="https://metatags.io/">Metatags.io</a> to generate meta tags for sharing your portfolio and for SEO benefits.  

## Styling
We are using plain `CSS` for this project and you can find that in the `docs/css/` folder
- style.css is the main file
- utilities.css is where reusable styling will be. 

<h1>Examples</h1>
<p>Here are examples of portfolios customized using this template, you can draw inspiration from this list or add yours.</p>

<table>
<tr>
<!-- Start of column-1 -->
<td>
  <a href="https://cpro-portfolio-html.netlify.app/">
    <img src="https://user-images.githubusercontent.com/62628408/150613011-b78a7f5a-0af1-4312-aab0-0022e7258693.png" width="100px"> <br/>
    <sub>Example 1</sub>
  </a>
</td>
<!-- End of column-1 -->
 <!-- Start of column-2 -->
<td>
  <a href="https://cpro-portfolio-html.netlify.app/">
    <img src="https://user-images.githubusercontent.com/62628408/150613011-b78a7f5a-0af1-4312-aab0-0022e7258693.png" width="100px"> <br/>
    <sub>Example 2</sub>
  </a>
</td>
</tr>
</table>



## Sponsor
<div>
  <a href="https://www.buymeacoffee.com/victoreke">
    <img width="150px" alt="bmc-button" src="https://user-images.githubusercontent.com/62628408/127788747-8850d386-fc61-4fff-b18f-8c5ee597be34.png">
  </a>
<img width="150px" height="100%" src="https://img.shields.io/badge/sponsor-30363D?style=for-the-badge&logo=GitHub-Sponsors&logoColor=#white">
</div>

If you like this project, kindly star ⭐ and share this project. It means the world to us.
You can also offer support by donating to keep this project going.
