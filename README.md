# AI Prompt Builder for Teachers

A user-friendly web application that helps educators create well-structured prompts for AI tools. Teachers can select from various generators, customize parameters, and generate professional prompts formatted for optimal AI responses.

## Features

### 🎯 Multiple Generator Types
- **Assessment Generator** - Create quizzes and tests with customizable question types and DOK levels
- **Lesson Designer** - Design detailed lesson plans with structure and differentiation options
- **Exit Ticket Generator** - Build quick formative assessments
- **Bell Ringer/Class Starter** - Generate engaging opening activities
- **Differentiation Builder** - Create tiered activities for diverse learners
- **Writing Prompt Creator** - Develop creative writing prompts
- **Concept Explanation** - Generate clear explanations for complex topics
- **Parent Email Template** - Draft professional parent communications
- **Grading Rubric** - Build detailed assessment rubrics

### ⚙️ Customization Options
- **Grade Level Selection** - Target specific high school grades (9-12)
- **Subject Areas** - Choose from core subjects, STEM, arts, and more
- **Reading Levels** - Adjust complexity from middle school to college level
- **DOK Levels** - Specify Depth of Knowledge requirements
- **Question Types** - Select from multiple choice, short answer, CER-style, and more
- **Lesson Components** - Include warm-ups, modeling, guided practice, and more
- **Differentiation Levels** - Add basic or detailed tiered instruction

### 📋 Structured Output
The tool generates prompts with clear sections:
- **ROLE** - Sets the AI's perspective as an educator
- **TASK** - Describes what to create
- **PARAMETERS** - Lists all selected options (DOK levels, question types, etc.)
- **FORMAT REQUIREMENTS** - Specifies output formatting needs
- **ADDITIONAL REQUIREMENTS** - Includes custom details and constraints

### ✨ User-Friendly Interface
- Clean, modern design with Tailwind CSS
- Real-time prompt generation as you select options
- One-click copy functionality
- Responsive layout for desktop and mobile
- Conditional options that appear based on generator selection
- Clear all button to start fresh

## How to Use

1. **Select a Generator** - Choose what type of content you want to create from the dropdown
2. **Choose Global Settings** - Select subject, grade level, reading level, and topic
3. **Configure Options** - Use the conditional options that appear for your chosen generator
4. **Add Custom Details** - Include any specific requirements or constraints
5. **Copy the Prompt** - Click the "Copy Prompt" button and paste into your AI tool

## File Structure

```
AI-Prompt-Builder-for-Teachers/
├── index.html          # Main application file (HTML, CSS, JavaScript)
├── README.md           # This file
└── lancer.png          # School logo image
```

## Installation

### Basic Setup
1. Clone or download this repository
2. Open `index.html` in any modern web browser
3. No server or dependencies required - it runs entirely in the browser!

### GitHub Pages Deployment
1. Push the repository to GitHub
2. Go to repository Settings → Pages
3. Select your branch (usually `main`) and root folder
4. Save and your site will be live at `https://[username].github.io/[repository-name]/`

### Customization

#### Change the Logo
Replace the logo URL in the HTML (line 39):
```html
<img id="school-logo" src="YOUR-LOGO-URL" alt="School Logo" class="h-12 w-12">
```

#### Modify Grade Levels
To add elementary or middle school options, edit the grade level dropdown (around line 232).

#### Add New Subjects
Add more subject options in the subject dropdown (around line 243).

#### Customize Reading Levels
Modify reading level descriptions in the reading level dropdown (around line 257).

#### Add Generator Types
To add a new generator:
1. Add an option to the task selector dropdown
2. Create a new conditional options block in the HTML
3. Add a new case in the `generatePrompt()` function in the JavaScript

## Technologies Used

- **HTML5** - Structure and content
- **Tailwind CSS** (CDN) - Styling and responsive design
- **Vanilla JavaScript** - Interactive functionality
- **Inter Font** - Typography

## Browser Compatibility

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Ideas for Contributions
- Add more generator types
- Include elementary/middle school grade levels
- Add more differentiation options
- Create preset templates for common use cases
- Add export functionality (PDF, Word, etc.)
- Include sample prompts/examples
- Add support for other languages

## License

This project is open source and available for educational use.

## Support

For questions, issues, or suggestions:
- Open an issue on GitHub
- Contact the maintainers
- Submit a pull request with improvements

## Acknowledgments

Built for teachers, by educators who understand the power of well-crafted prompts in AI-assisted instruction.

---

**Note**: This tool generates prompts for use with AI assistants (like ChatGPT, Claude, Gemini, etc.). You'll need to copy the generated prompt and paste it into your preferred AI tool - this application does not directly connect to any AI APIs.
