# E-Pathshala – India's All-Board Learning Hub

Welcome to **E-Pathshala**, a comprehensive online learning platform designed to serve students across different Indian educational boards. This platform provides an interactive and elegant interface for accessing educational content tailored to various curricula including CBSE, ICSE, NIOS, and State Boards.

## 🎓 Features

- **Multi-Board Support**: Access resources for CBSE, ICSE, NIOS, and State Board curricula
- **AI-Powered Learning**: Integration with Google Gemini API for intelligent tutoring and content recommendations
- **Elegant User Interface**: Beautiful, regal design with smooth navigation and intuitive layout
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Fast Performance**: Lightweight static HTML files served efficiently via Node.js

## 📋 Project Structure

```
.
├── landing.html          # Home page with platform overview
├── cbse.html            # CBSE board curriculum resources
├── icse.html            # ICSE board curriculum resources
├── nios.html            # NIOS board curriculum resources
├── state-board.html     # State board curriculum resources
├── server.js            # Node.js HTTP server
├── package.json         # Project metadata and dependencies
├── metadata.json        # Application configuration
└── README.md            # This file
```

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v12 or higher)
- **npm** (comes with Node.js)
- **Gemini API Key** (for AI-powered features)

### Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd E-Pathshala-final
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Set up environment variables**:
   - Create a `.env.local` file in the root directory
   - Add your Gemini API key:
     ```
     GEMINI_API_KEY=your_gemini_api_key_here
     ```

### Running the Application

#### Development Mode

```bash
npm run dev
```

The application will start on `http://localhost:3000`

#### Production Mode

```bash
npm start
```

### Building for Deployment

```bash
npm run build
```

This command creates a `dist/` directory with all necessary files ready for deployment.

## 📖 Usage

### Accessing Different Board Resources

- **Home/Landing Page**: http://localhost:3000/
- **CBSE Resources**: http://localhost:3000/cbse.html
- **ICSE Resources**: http://localhost:3000/icse.html
- **NIOS Resources**: http://localhost:3000/nios.html
- **State Board Resources**: http://localhost:3000/state-board.html

## 🛠️ Technical Details

### Server Configuration

The application uses a custom Node.js HTTP server (`server.js`) that:
- Serves static HTML, CSS, and JavaScript files
- Routes the root path (`/`) to `landing.html`
- Handles 404 errors gracefully
- Supports multiple MIME types for various file formats

### Supported File Types

- HTML, CSS, JavaScript
- Images: PNG, JPG, GIF, SVG, ICO
- JSON files
- And more as configured in `server.js`

## 🔧 Development

### Adding New Pages

1. Create a new `.html` file in the root directory
2. Access it via `http://localhost:3000/your-page.html`
3. Update the build script in `package.json` if deploying

### Customization

- Modify the port number in `server.js` (currently set to 3000)
- Update styling in the HTML files using the regal color scheme
- Integrate Gemini API calls for AI-powered features

## 📝 Available Scripts

| Script | Description |
|--------|-------------|
| `npm run dev` | Start the development server on port 3000 |
| `npm start` | Start the production server |
| `npm run build` | Build the application for deployment |
| `npm run lint` | Run linting checks (currently disabled) |

## 🌐 Deployment

### Deploy to Vercel, Netlify, or Any Node.js Hosting

1. Run `npm run build` to create the `dist/` directory
2. Deploy the contents of the `dist/` directory (or entire project directory)
3. Ensure `server.js` is executed as the start command
4. Set the `GEMINI_API_KEY` environment variable on your hosting platform

### Example (Vercel):
```bash
npm run build
vercel --prod
```

## 🎨 Design Philosophy

E-Pathshala features a sophisticated, regal design with:
- **Color Palette**: Gold accents, maroon, saffron, and cream backgrounds
- **Typography**: Poppins and Playfair Display fonts
- **Visual Effects**: Smooth animations, shimmer effects, and elegant spacing
- **Accessibility**: Clear contrast and responsive layouts

## 🐛 Troubleshooting

### Port Already in Use

If port 3000 is already in use, modify the `PORT` variable in `server.js`:
```javascript
const PORT = 3001; // or any available port
```

### Missing Dependencies

Run `npm install` again to ensure all dependencies are properly installed.

### API Errors

Verify that your `GEMINI_API_KEY` is correctly set and valid. Check the error logs in the terminal for more details.

## 📄 License

This project is part of the E-Pathshala initiative for educational technology in India.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests with improvements, bug fixes, or new features.

## 📧 Support

For questions or issues, please open an issue in the repository or contact the development team.

---

**Made with ❤️ for India's students**
