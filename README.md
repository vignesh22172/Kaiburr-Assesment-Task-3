# Kaiburr-Assesment-Task-3
# 🚀 Web UI Frontend

[![React](https://img.shields.io/badge/React-18.2.0-blue.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.2.2-blue.svg)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.0.8-646CFF.svg)](https://vitejs.dev/)
[![Ant Design](https://img.shields.io/badge/Ant%20Design-5.12.8-1890FF.svg)](https://ant.design/)


A modern, accessible React + TypeScript frontend application for managing records and running commands with live output. Built with enterprise-grade UI components and comprehensive accessibility features.


![Demo](demo.gif)
![Image](https://github.com/user-attachments/assets/e07dcc2a-1a8a-4d07-b8a9-60ee9f0e5773)

## ✨ Features

### 🗃️ Records Management
- ✅ **Create** new records with validation
- ✅ **View** all records in a responsive, sortable table
- ✅ **Search** records by name or description with real-time filtering
- ✅ **Edit** existing records with modal forms
- ✅ **Delete** records with confirmation dialogs
- ✅ **Sort** by name, creation date, or update date
- ✅ **Pagination** with customizable page sizes

### ⚡ Commands Runner
- ✅ **Execute** commands with custom names
- ✅ **Monitor** command status (running, completed, failed, stopped)
- ✅ **View** live command output in terminal-style interface
- ✅ **Real-time updates** every 2 seconds for running commands
- ✅ **Stop** running commands with confirmation
- ✅ **Delete** completed commands
- ✅ **Copy** commands to clipboard

### ♿ Accessibility (WCAG 2.1 AA Compliant)
- ✅ **ARIA labels** and descriptions for screen readers
- ✅ **Keyboard navigation** support for all interactive elements
- ✅ **High contrast** focus indicators
- ✅ **Semantic HTML** structure
- ✅ **Screen reader** announcements for dynamic content

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| **React** | 18.2.0 | UI Framework |
| **TypeScript** | 5.2.2 | Type Safety |
| **Vite** | 5.0.8 | Build Tool |
| **Ant Design** | 5.12.8 | UI Components |
| **React Router** | 6.20.1 | Navigation |
| **Axios** | 1.6.2 | API Communication |
| **Day.js** | 1.11.10 | Date Formatting |

## 🚀 Quick Start

### Prerequisites
- **Node.js** 16+ 
- **npm** or **yarn**

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/web-ui-frontend.git
   cd web-ui-frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure API endpoint (optional):**
   ```bash
   cp .env.example .env
   # Edit .env to set VITE_API_BASE_URL if needed
   ```

4. **Start development server:**
   ```bash
   npm run dev
   ```

5. **Open your browser:**
   Navigate to `http://localhost:3000`

### 🏗️ Build for Production

```bash
npm run build
npm run preview
```

## 📱 Demo

Try the live demo: [Web UI Frontend Demo](https://your-demo-url.com)

### Sample Data
The application includes mock data for testing when no backend API is available:
- **Sample Records:** Documentation, bug reports, feature requests
- **Sample Commands:** File operations, system commands

## 🔧 API Configuration

The application works with a backend API or uses mock data as fallback:

| Configuration | Value | Description |
|---------------|-------|-------------|
| **API Base URL** | `VITE_API_BASE_URL` | Environment variable |
| **Default** | `http://localhost:8000` | Default API endpoint |
| **Fallback** | Mock data | Used when API unavailable |

### 📡 API Endpoints

<details>
<summary><strong>Records API</strong></summary>

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/records` | List records with pagination and search |
| `GET` | `/records/:id` | Get single record |
| `POST` | `/records` | Create new record |
| `PUT` | `/records/:id` | Update record |
| `DELETE` | `/records/:id` | Delete record |

</details>

<details>
<summary><strong>Commands API</strong></summary>

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/commands` | List all commands |
| `GET` | `/commands/:id` | Get single command |
| `POST` | `/commands` | Start new command |
| `POST` | `/commands/:id/stop` | Stop running command |
| `DELETE` | `/commands/:id` | Delete command |

</details>

## Project Structure

```
src/
├── components/
│   └── Layout/
│       └── AppLayout.tsx      # Main application layout
├── pages/
│   ├── Records.tsx            # Records management page
│   └── Commands.tsx           # Commands runner page
├── services/
│   └── api.ts                 # API service layer with mock fallback
├── App.tsx                    # Main app component with routing
├── main.tsx                   # Application entry point
└── index.css                  # Global styles and accessibility improvements
```

## Key Features

### Records Page
- **Responsive table** with sorting and pagination
- **Advanced search** with real-time filtering
- **Modal forms** for creating and editing
- **Confirmation dialogs** for destructive actions
- **Loading states** and error handling

### Commands Page
- **Real-time status updates** for running commands
- **Live output streaming** with auto-scroll
- **Command history** with timestamps
- **Terminal-style output** display
- **Copy-to-clipboard** functionality

### Accessibility
- **WCAG 2.1 AA compliant** design patterns
- **Screen reader** optimized
- **Keyboard-only** navigation support
- **Focus management** in modals
- **Semantic markup** throughout

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test accessibility with screen readers
5. Submit a pull request


