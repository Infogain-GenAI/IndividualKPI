# 📊 Nbly Digital Individual KPI Dashboard

An interactive web-based dashboard for visualizing and tracking individual Key Performance Indicators (KPIs) with sparkline charts, filtering capabilities, and expand/collapse functionality.

## 🎯 Purpose

This HTML dashboard is designed to:
- **Visualize KPI compliance** across multiple sprints using interactive sparkline charts
- **Track performance trends** with visual indicators (up/down/stable)
- **Filter and organize** KPIs by team, resource type, or compliance status
- **Provide interactive exploration** with collapsible sections and hover tooltips
- **Display compliance rates** with color-coded badges and issue tracking

## 🌐 Live Dashboard

The dashboard is published at: **https://infogain-genai.github.io/IndividualKPI/**

## 📁 Files

- `NblyIndividualTracker.html` - Main dashboard file with all functionality
- `index.html` - Redirect page for clean URL access
- `README.md` - This documentation

## 📋 How to Use

### 1. JSON Data Format

The dashboard expects JSON data in the following structure:

```json
{
  "TeamName/ResourceType": {
    "Resource1": {
      "Sprint1": 1,
      "Sprint2": 0,
      "Sprint3": 1,
      "Sprint4": 1
    },
    "Resource2": {
      "Sprint1": 0,
      "Sprint2": 1,
      "Sprint3": 0,
      "Sprint4": 1
    }
  }
}
```

### 2. Data Structure Explanation

- **Top Level Keys**: Represent KPI categories (e.g., "Development Team/Code Quality", "QA Team/Test Coverage")
- **Resource Names**: Individual resources being tracked (e.g., "UserService.java", "PaymentAPI.js")
- **Sprint Values**: Binary values where:
  - `1` = Compliant/Met KPI target (green)
  - `0` = Non-compliant/Missed KPI target (red)

### 3. Example JSON Data

```json
{
  "Development Team/Code Quality": {
    "UserService.java": {
      "Sprint 1": 1,
      "Sprint 2": 1,
      "Sprint 3": 0,
      "Sprint 4": 1,
      "Sprint 5": 1
    },
    "PaymentAPI.js": {
      "Sprint 1": 0,
      "Sprint 2": 1,
      "Sprint 3": 1,
      "Sprint 4": 0,
      "Sprint 5": 1
    },
    "DatabaseLayer.py": {
      "Sprint 1": 1,
      "Sprint 2": 1,
      "Sprint 3": 1,
      "Sprint 4": 1,
      "Sprint 5": 0
    }
  },
  "QA Team/Test Coverage": {
    "Unit Tests": {
      "Sprint 1": 1,
      "Sprint 2": 0,
      "Sprint 3": 1,
      "Sprint 4": 1,
      "Sprint 5": 1
    },
    "Integration Tests": {
      "Sprint 1": 0,
      "Sprint 2": 0,
      "Sprint 3": 1,
      "Sprint 4": 1,
      "Sprint 5": 1
    }
  },
  "Security Team/Vulnerability Assessment": {
    "Web Application Scan": {
      "Sprint 1": 1,
      "Sprint 2": 1,
      "Sprint 3": 1,
      "Sprint 4": 0,
      "Sprint 5": 1
    },
    "API Security Check": {
      "Sprint 1": 1,
      "Sprint 2": 1,
      "Sprint 3": 0,
      "Sprint 4": 1,
      "Sprint 5": 1
    }
  }
}
```

### 4. Using the Dashboard

1. **Input Data**: Paste your JSON data into the text area at the top
2. **Generate Charts**: Click "🔄 Generate Charts" to visualize the data
3. **Filter Data**: Use the dropdown to filter by team, compliance status, or view all
4. **Expand/Collapse**: 
   - Click on any KPI section header to expand/collapse
   - Use "Expand All" or "Collapse All" buttons for bulk actions
5. **Interactive Elements**:
   - Hover over sparkline points to see sprint details
   - View compliance rates and trend indicators
   - See issue counts for non-compliant resources

### 5. Dashboard Features

- **📈 Sparkline Charts**: Visual representation of KPI compliance over time
- **🎯 Compliance Rates**: Percentage-based performance indicators
- **📊 Trend Analysis**: Up/down/stable trend indicators
- **🔍 Filtering**: Filter by team, compliance status, or issues
- **📱 Responsive Design**: Works on desktop and mobile devices
- **🎨 Interactive UI**: Smooth animations and hover effects

## 🛠️ Customization

The dashboard can be customized by modifying:
- **Color schemes** in the CSS section
- **Compliance thresholds** in the JavaScript functions
- **Sprint column headers** (automatically detected from JSON)
- **Filtering options** in the dropdown menus

## 📊 Supported KPI Types

The dashboard works with any binary KPI metrics, such as:
- Code quality compliance
- Test coverage targets
- Security scan results
- Documentation completeness
- Performance benchmarks
- Process adherence
- Review completion rates

## 🚀 Deployment

This dashboard is automatically deployed via GitHub Pages and updates whenever changes are pushed to the main branch.
