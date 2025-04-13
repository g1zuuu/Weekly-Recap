# Weekly-Recap

# Web Programming Basics – Notes (Meetings 1–7)

## 📘 Meeting 1 – Computer Networks, Internet, and Web Technology

### Learning Goals
- Understand and analyze computer network concepts, the internet, and web technology.
- Recognize the difference between static and dynamic websites.

### Key Concepts

#### 1. Computer Networks & Internet ( Basic )
- Internet: Global interconnection of IP-based networks (IPv4 & IPv6).
- Internet Applications: All run on protocols (e.g., HTTP/HTTPS, FTP, SMTP). Example: Web (WWW).

#### 2. www stands for World Wide Web (Web)
- A system of digital information (text, images, audio, video) accessed via browsers using **HTTP/HTTPS**.
- Web Pages: Presented in hypertext format; accessed on port 80 (HTTP).

#### 3. Types of Websites
- Static Web: Fixed pages; content edited manually via source code.
- Dynamic Web: Content changes frequently; connected to a database and allows user interaction.
- Jamstack: JavaScript, API, Markup.

#### 4. History of the Web
- 1960s: ARPANET by the U.S. Dept. of Defense.
- 1989: Tim Berners-Lee invented WWW with HTTP, HTML, URL.
- 1993: Mosaic browser introduced image support.
- Late 1990s: Dot-com boom; rise of Yahoo!, Amazon.

#### 5. Web Programming
- Client-Side: HTML, CSS, JavaScript (executed in browser) → static.
- Server-Side: PHP, ASP, JSP, NodeJS (executed on server).

#### 6. Web Categories
- Personal Website: Managed by individuals (WordPress, Blogger).
- Business Website: For company branding and profile.
- Community Website: For discussions, campaigns, often ends in `.org`.

#### 7. Web Technology Overview
- **Frontend vs Backend**
- **Web Server**: Software that handles requests (Apache, Nginx, etc.)

#### 8. Important Web Technologies (Discussion Topics)
- DNS, SSL, CDN, HTTP3, Web3, SEO, Caching, Cookies, Meta Description, Serverless, Backendless
  
---

## Meeting 2 – Tech Stack & Web Environment

### Learning Goals
- Understand frontend, backend, and full-stack development.
- Analyze web applications, programming languages, and dev tools (tech stack).

### Key Concepts

#### 1. Frontend vs Backend
- Frontend: Visible part of the app (UI/UX), runs in browser.
- Backend: Server-side logic, database interaction.

#### 2. Full Stack = Frontend + Backend

#### 3. Tech Stack (Solution Stack)
- Combination of tools & technologies to build/run apps.
- Includes OS, languages, frameworks, DBs, analytics, monitoring, etc.

#### 4. Example Tech Stacks
- **MEVN**: MongoDB, Express.js, Vue.js, Node.js
- **MERN**: MongoDB, Express.js, React.js, Node.js
- **LAMP**: Linux, Apache, MySQL, PHP
- **Jamstack**: JavaScript, API, Markup

--- 

## Meetings 3–4 – HTML5

### Learning Goals
- Apply and create basic HTML5 structure and elements.

### Key Concepts

#### 1. What is HTML?
- Markup language (not programming) used to build web pages.
- Created by Tim Berners-Lee (1991); current standard maintained by W3C.

#### 2. HTML5
- Introduced in 2014, widely supported by browsers.
- Improves semantics, accessibility, SEO, and functionality.
- Supports new APIs: Canvas, Geolocation, Video/Audio, Local Storage, etc.

#### 3. Semantic Elements
- `<header>`, `<nav>`, `<section>`, `<article>`, `<aside>`, `<footer>`
- Improves structure, SEO, and screen reader access.

a. <header>
- Purpose: Defines introductory content like logo, title, navigation.
- Example:
<header>
  <h1>My Website</h1>
  <p>Welcome to my page!</p>
</header>

<nav>
Example:
<nav>
- Purpose: Contains navigation links.
<nav>
  <a href="#about">About</a> |
  <a href="#courses">Courses</a>
</nav>
  
<section>
- Purpose: Groups related content (e.g., sections of a page).
- Example:
<section id="about">
  <h2>About</h2>
  <p>This section contains info about the website.</p>
</section>
  
<article>
- Purpose: Represents self-contained content (like blog posts, news).
- Example:
<article>
  <h2>Blog Title</h2>
  <p>Written by Author</p>
</article>
  
<aside>
- Purpose: Side content related to the main page (ads, tips).
- Example:
<aside>
  <h3>Tip of the Day</h3>
  <p>Use semantic tags for better SEO.</p>
</aside>
  
<footer>
- Purpose: Defines footer info like copyright.
- Example:
<footer>
  <p>&copy; 2025 My Website</p>
</footer>

#### 4. HTML vs HTML5
- HTML5 supports SVG, Canvas, LocalStorage, modern form controls (date, email, etc.)

---

## Meetings 5–7 – CSS3

### Learning Goals
- Apply basic CSS3 styling for web design.

### Key Concepts

#### 1. What is CSS?
- CSS stands for Cascading Style Sheets: Style language to design HTML elements.

#### 2. CSS Syntax
```css
selector {
  property: value;
}
```

#### 3. Types of CSS Usage
- External: Link external `.css` file in `<head>`
- Internal: Use `<style>` tag in `<head>`
- Inline: Add `style="..."` directly to HTML tag
- Multiple: Combine external, internal, and inline styles

Detailed Explanation of the 4 types of CSS Usage: Inline, Internal, External, Multiple
Detailed Types of CSS Usage
1. External CSS
What: CSS is placed in a separate .css file.
Why: Ideal for reusing styles across multiple HTML pages.
How: Link it in the <head> section using <link> tag.

Example:
in file named "style.css", written:
body {
  background-color: lightgray;
} 
in file named "index.html", written:
<head>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>

Note: The <link href tag is used to assign the CSS setup set in the file named style.css, or any other names written in the href field. Keyword: Link, <link>, separated structure and styling files.


2. Internal CSS
What: CSS is written inside a <style> tag in the <head> of the HTML file.
Why: Useful when styling is only applied to a single page.
Example:
in file named "index.html", written:
<head>
  <style>
    h1 {
      color: darkblue;
      font-size: 32px;
    }
  </style>
</head>

Note: The <style> tag is used inside the <head> section of the HTML file to embed CSS directly in the document. This method is suitable when you want the styling to affect only that specific page.
Keyword: Internal, <style>, page-specific styling.

3. Inline CSS
What: CSS is written directly in the element using the style attribute.
Why: Best for quick, one-time, specific element styling.
Example:
<p style="color: green; background-color: beige;">This is styled inline</p>

Note: : The style attribute is used directly within an HTML tag to apply specific styling. Not ideal for maintainability in large-scale projects, as changes would need to be repeated manually across multiple tags instead of being centralized in a stylesheet.


4. Multiple Style Sheets
What: Combines external, internal, and inline styles.
Why: Useful for layering styles, but be careful with specificity and override rules.

Example:
<!-- External -->
<link rel="stylesheet" href="base-style.css">

<!-- Internal -->
<style>
  p {
    font-family: Arial;
  }
</style>

<!-- Inline -->
<p style="color: red;">Inline wins in specificity if not overridden!</p>

Note: When multiple CSS types are used together, they cascade based on specificity and order. Inline styles have the highest priority, followed by internal, and then external. 

#### 4. CSS Capabilities
- Font, size, layout, color, responsiveness, form styling
- Compatible with all modern browsers


