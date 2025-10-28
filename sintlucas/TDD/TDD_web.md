I will edit this document more a little bit later on
# Technical Design Document for Software Developer Portfolio Website
This document provides technical details based on the provided functional design document. 
It outlines the system architecture, components, and technology stack used to build and maintain the website.

## System Architecture
The front end will be served as a single-page application (SPA) for a fluid user experience.
There will be no backend.
![architecture_simple.png](images%2Farchitecture_simple.png)


---

### General idea for the website flow
- **Land page (business card style):**
    - Name
    - Buttons that lead to other main pages (→About →Contact →Project)
    - “logo” aka pfp
    - “job title” aka a tiny description of either this website or me like “SD student, spezialize in Web Dev”
- **About page:**
    - Some text about me as a person
    - Some text about me as a developer
    - Some text about my other interests
    - Timeline
    - Language proficiency table
    - Dev tools proficiency table/mention
- **Projects page (page showcasing all the projects)**
    - Project containers (onclick of which leads to a dedicated page w/more info → Project pages)
        - Image/video/gif
        - Name of project
        - Tools used to make it
    - Button/link that leads the user to the page where games I mentioned can be played thought WebGL
- **Project pages (page per project)**
    - Image/video/gif
    - Name of project
    - Tools used to make it
    - Text about why it was made
    - Text about how it was made
    - Text about which skills I learned from making it
    - Link GitHub repository of the project
- **Contact page**
    - Email
    - Phone number (maybe)
    - LinkedIn when I make one maybe (future, not now)
    - GitHub profile (but a new one! not a school one)
    - Time zone mention (not a priority)

---

### Frontend
- **Technology:** HTML/CSS, JavaScript without any frameworks.
- **Styling:** CSS Flexbox and CSS Grid. The styling adapts to different screen sizes (mobile vs desktop).

### Deployment
- **Servers:** Deployed on Github Pages (or SaaS (Software as a Service) platform like Render.com).
- **CI/CD:** When using Render.com, continuous deployment will be implemented using their built-in GitHub integration.

## Security Considerations
- **HTTPS:** All traffic will be served over HTTPS to ensure data integrity and confidentiality.

## Testing
- **IDE:** Used to prevent syntax errors or runtime errors.
- **User Testing:** User testing will be conducted to ensure the application is user-friendly and meets user expectations.
- **Cross-Browser Testing:** The application will be tested on multiple browsers (Chrome, Firefox, Safari, Edge) to ensure compatibility.
- **Performance Testing:**: The application will be tested with Google Chromes Lighthouse to ensure fast loading times and optimal performance.
