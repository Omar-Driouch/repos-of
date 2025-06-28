# 🚀 GitHub Portfolio Browser

A beautiful, responsive web application that displays GitHub repositories in an elegant portfolio format. Perfect for showcasing your coding projects with style!

## ✨ Features

- 🎨 **Modern Design**: Clean, responsive interface with smooth animations
- 📊 **Project Stats**: Shows stars, forks, last updated date, and repository size
- 🏷️ **Language Tags**: Displays the primary programming language for each project
- 📄 **Pagination**: Easy navigation through multiple pages of repositories
- 🌐 **Live Demo Links**: Direct links to project demos and issue tracking
- 🎯 **URL Parameters**: Easy user switching via URL parameters

## 🎬 Live Demo

[View Live Demo](https://omar-driouch.github.io/repos-of/)

## 📸 Screenshots

![GitHub Portfolio Browser Screenshot](https://i.ibb.co/LhB9MP2c/Capture-d-cran-2025-06-28-214534.png)
![GitHub Portfolio Browser Screenshot](https://i.ibb.co/7JdmWtnK/Capture-d-cran-2025-06-28-215047.png)
## 🛠️ Installation & Setup

### Method 1: Quick Start (Recommended)

1. **Download the HTML file**
   ```bash
   # Clone this repository
   git clone https://github.com/your-username/github-portfolio-browser.git
   
   # Or download the HTML file directly
   wget https://raw.githubusercontent.com/your-username/github-portfolio-browser/main/index.html
   ```

2. **Customize the default username**
   - Open the HTML file in a text editor
   - Find line with `return urlParams.get('user') || 'Omar-Driouch';`
   - Replace `'Omar-Driouch'` with your GitHub username
   ```javascript
   return urlParams.get('user') || 'YOUR-GITHUB-USERNAME';
   ```

3. **Open in browser**
   - Simply double-click the HTML file
   - Or serve it using a local server



## 🎯 Usage Guide

### Basic Usage

The application will automatically load with your default username. No configuration needed!

### Switching Users

**URL Parameters (Recommended)**
```
https://yourdomain.com/?user=octocat
https://yourdomain.com/?user=microsoft
https://yourdomain.com/?user=omar-driouch
```



## 🌐 Integration with Your Portfolio

### Option 1: Standalone Page

1. **Add to your existing website**
   ```html
   <!-- In your main portfolio -->
   <a href="github-portfolio.html" class="portfolio-link">
     🚀 View My GitHub Projects
   </a>
   ```

2. **Create a dedicated section**
   ```html
   <section id="github-projects">
     <h2>My GitHub Portfolio</h2>
     <iframe src="github-portfolio.html" width="100%" height="800px"></iframe>
   </section>
   ```



### Option 2: Embed in Existing Portfolio

1. **As a section in your main portfolio**
   ```html
   <section class="github-section">
     <div class="container">
       <h2>My GitHub Projects</h2>
       <div id="github-embed">
         <!-- Paste the body content of the GitHub portfolio here -->
       </div>
     </div>
   </section>
   ```

2. **Include the CSS and JavaScript**
   ```html
   <head>
     <!-- Your existing head content -->
     <style>
       /* Paste the GitHub portfolio CSS here */
     </style>
   </head>
   
   <body>
     <!-- Your portfolio content -->
     
     <script>
       /* Paste the GitHub portfolio JavaScript here */
     </script>
   </body>
   ```

## ⚙️ Customization Options

### Changing Default Settings

1. **Default Username**
   ```javascript
   // Line ~290
   return urlParams.get('user') || 'YOUR-USERNAME';
   ```

2. **Projects Per Page**
   ```javascript
   // Line ~280
   let projectsPerPage = 6; // Change to 9, 12, etc.
   ```

 

### Styling Customization

1. **Color Scheme**
   ```css
   /* Change primary color */
   --primary-color: #4f46e5; /* Replace with your brand color */
   
   /* Update gradient background */
   background: linear-gradient(to bottom right, #your-colors);
   ```

2. **Typography**
   ```css
   /* Change font family */
   font-family: 'Your-Font', sans-serif;
   ```

3. **Card Layout**
   ```css
   /* Adjust card sizing */
   .projects-grid {
     grid-template-columns: repeat(auto-fit, minmax(400px, 1fr)); /* Larger cards */
   }
   ```

 
## 🔧 Troubleshooting

### Common Issues

**1. Rate Limit Exceeded**
```
Error: GitHub API rate limit exceeded
Solution: Wait 1 hour or use a different network
```

**2. User Not Found**
```
Error: User 'username' not found
Solution: Check spelling and ensure the GitHub username exists
```

**3. No Repositories Showing**
```
Possible causes:
- User has no public repositories
- All repositories are forks (filtered out by default)
- Network connectivity issues
```




## 📞 Support


- 📧 [**LinkedIn**: ](https://www.linkedin.com/in/omar-driouch/)

---

**Made with ❤️ by [OMAR DRIOUCH](https://github.com/Omar-driouch)**

⭐ If you found this project helpful, please give it a star on GitHub!
