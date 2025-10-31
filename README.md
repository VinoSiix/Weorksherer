# 📚 Worksheet Generator

An AI-powered educational tool that creates custom worksheets instantly. Generate grade-specific worksheets with AI assistance, convert them to professional PDFs, and manage your entire worksheet history.

## ✨ Features

- **🎓 Grade-Specific Content**: Worksheets tailored for grades Kindergarten through 12th grade
- **🤖 AI-Powered Generation**: Advanced AI creates high-quality educational content
- **📄 Professional PDFs**: Get separate PDF downloads for questions and answers
- **🔖 Markdown Support**: Bold text formatting in generated worksheets using **text**
- **📋 Interactive Form**: Easy customization with subject, topic, difficulty, and extra details
- **🗂️ Worksheet History**: Comprehensive history management and organization
- **👥 User Authentication**: Secure account-based worksheet management via Supabase
- **🎨 Modern UI**: Beautiful, responsive interface with dark/light theme support
- **⚡ Instant Generation**: Get worksheets in seconds with real-time AI processing

## 🚀 Quick Start

### Prerequisites
- Node.js & npm installed ([install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating))

### Installation

```bash
# Clone the repository
git clone <YOUR_GIT_URL>
cd worksheet-generator

# Install dependencies
npm install

# Start development server
npm run dev
```

### Environment Setup
Create a `.env` file in the root directory:

```env
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

## 🏗️ Tech Stack

- **Frontend**: React 18 + TypeScript + Vite
- **UI**: shadcn/ui components + Tailwind CSS
- **Backend**: Supabase (Authentication & Database)
- **PDF Generation**: jsPDF (client-side PDF creation)
- **Icons**: Lucide React
- **Routing**: React Router v6

## 📁 Project Structure

```
/src
├── components/          # Reusable UI components
│   ├── Header.tsx       # Global navigation header
│   └── ui/              # shadcn/ui components
├── pages/               # Application routes
│   ├── Auth.tsx         # Authentication page
│   ├── Generator.tsx    # Worksheet generation form
│   ├── History.tsx      # Worksheet history management
│   └── Landing.tsx      # Landing page with features
├── integrations/        # External service integrations
└── lib/                 # Utility functions
```

## 🎯 Usage

### 1. **Generate Worksheets**
- Navigate to the Generator page
- Select grade level, subject, and enter topic
- Adjust difficulty and question count
- Add extra details for customization
- Enable answer key if needed

### 2. **AI-Powered Creation**
- Content is generated via n8n workflows
- Text is processed and converted to professional PDFs
- **Bold text** support for markdown formatting

### 3. **Manage History**
- Access all generated worksheets from the History page
- Download questions and answers separately
- View creation timestamps and details
- Search and organize your content

### 4. **PDF Features**
- Professional formatting with grade/subject headers
- Separate question and answer sheets
- Clean, printable layouts
- Instant download functionality

## 🎨 Customization

### Adding New Grade Levels
Edit the `grades` array in `Generator.tsx`:

```typescript
const grades = [
  "Kindergarten",
  "1st Grade",
  // ... add new grades
];
```

### Adding New Subjects
Update the `subjects` array:

```typescript
const subjects = [
  "Math",
  "Science",
  // ... add new subjects
];
```

### Styling
- **Themes**: Built-in light/dark mode support
- **Colors**: Wine red accent color with comprehensive color palette
- **Animations**: Smooth hover effects and transitions
- **Responsive**: Mobile-first design approach

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -m 'Add feature'`
4. Push: `git push origin feature-name`
5. Open a Pull Request

## 🐛 Troubleshooting

### Common Issues

**PDF Generation Issues:**
- Ensure jsPDF is properly installed
- Check for network connectivity to AI services

**Authentication Problems:**
- Verify Supabase configuration
- Check environment variables

**Styling Issues:**
- Clear Tailwind cache: `npx tailwindcss -i ./src/index.css -o ./dist/output.css --watch`
- Rebuild node_modules if needed

### Development Commands

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Run linting
npm run lint

# Preview production build
npm run preview
```

## 📜 License

This project is proprietary software. All rights reserved.

## 📞 Support

For technical support or questions:
- Open an issue in the GitHub repository
- Include your error logs and environment details
- Describe the steps to reproduce any issues

---

**Made with ❤️ for educators worldwide**
