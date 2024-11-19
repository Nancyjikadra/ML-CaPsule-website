# ML-Capsule Website  

This project is a responsive and dynamic website designed to showcase machine learning projects as part of the **GirlScript Summer of Code (GSSoC) 2024**. The website fetches project data directly from GitHub using API integration, providing users with easy access to project repositories. Built with modern web technologies, the website ensures a seamless and visually appealing user experience.

---

## Features  

### 🎨 **Responsive Design**  
- Built with **HTML**, **CSS**, **JavaScript**, and **Tailwind CSS** to ensure a smooth and consistent experience across various devices and screen sizes.  

### 🔗 **GitHub API Integration**  
- Dynamically fetches project links from GitHub repositories using the GitHub REST API.  
- Projects are displayed in an organized and user-friendly manner.  

### 🌟 **Enhanced User Experience**  
- Fast loading times with optimized CSS and JavaScript.
- Clean and intuitive interface that enhances accessibility and usability.  

---

## Tech Stack  

| Technology      | Description                                         |  
|------------------|-----------------------------------------------------|  
| **HTML**        | Structure and semantic layout of the website.        |  
| **CSS**         | Styling for enhanced visual appeal.                  |  
| **JavaScript**  | Adds interactivity and functionality.                |  
| **Tailwind CSS**| Utility-first CSS framework for responsive design.   |  
| **GitHub API**  | Fetches project details dynamically.                 |  

---

## Installation  

Follow these steps to set up the project locally:  

1. **Clone the repository:**  
   ```bash  
   git clone https://github.com/Nancyjikadra/ML-CaPsule-website.git  
   cd <repository-name>  
   ```  

2. **Open the project:**  
   - Simply open the `index.html` file in your browser to view the website.  

3. **Fetch GitHub project data:**  
   - Replace the placeholder `GitHub API Token` in the JavaScript file (`script.js`) to authenticate API calls.  

---

## Usage  

1. **Homepage:**  
   - The homepage showcases a visually appealing layout of the ML-Capsule projects.  
   - Each project card dynamically fetches its title and repository link from GitHub.  

2. **Navigation:**  
   - Easy-to-use navigation bar for smooth browsing.  

3. **Explore Projects:**  
   - Click on any project link to navigate to its GitHub repository for more details.  

---

## GitHub API Integration  

To integrate GitHub API:  

1. Create a GitHub personal access token:  
   - Navigate to your GitHub account settings.  
   - Go to **Developer Settings > Personal Access Tokens > Tokens (classic)**.  
   - Generate a token with the required permissions.  

2. Replace the placeholder in `script.js`:  
   ```javascript  
   const GITHUB_API_TOKEN = '<Your GitHub API Token>';  
   ```  

3. Fetch projects dynamically using:  
   ```javascript  
   fetch('https://api.github.com/users/<username>/repos', {  
       headers: {  
           Authorization: `token ${GITHUB_API_TOKEN}`  
       }  
   })  
   .then(response => response.json())  
   .then(data => displayProjects(data));  
   ```  

---

## Contributions  

Contributions are welcome! To contribute:  

1. Fork the repository.  
2. Create a new feature branch.  
   ```bash  
   git checkout -b feature/your-feature-name  
   ```  
3. Commit your changes.  
   ```bash  
   git commit -m "Add your message here"  
   ```  
4. Push your branch.  
   ```bash  
   git push origin feature/your-feature-name  
   ```  
5. Open a pull request on GitHub.  

---

## License  

This project is licensed under the [MIT License](LICENSE).  

---

## Acknowledgements  

- **GirlScript Summer of Code (GSSoC) 2024** for the opportunity to contribute and collaborate.  
- The amazing contributors and mentors who made this project possible.  

