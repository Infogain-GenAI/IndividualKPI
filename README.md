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

The dashboard is published at: ** https://infogain-genai.github.io/IndividualKPI/**

## 📁 Files

- `NblyIndividualTracker.html` - Main dashboard file with all functionality
- `index.html` - Redirect page for clean URL access
- `README.md` - This documentation

## 📋 How to Use

### 1. JSON Data Format

The dashboard expects JSON data in the following structure:

```json
[
  {
    "Resource": "Ajay Varma <ajaykumar.s@org.com>",
    "KPI Name": "Ado Hygiene",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "Ajay Varma <ajaykumar.s@org.com>",
    "KPI Name": "Daily Burndown for Tasks",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "Ajay Varma <ajaykumar.s@org.com>",
    "KPI Name": "Defects introduced - Dev/QA",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "vivek.jain <vivek.jain@org.com>",
    "KPI Name": "Ado Hygiene",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "vivek.jain <vivek.jain@org.com>",
    "KPI Name": "Daily Burndown for Tasks",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "vivek.jain <vivek.jain@org.com>",
    "KPI Name": "Defects introduced - Dev/QA",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  }
]
```

### 2. Data Structure Explanation

- **Top Level Keys**: Represent KPI categories (e.g., "Ado Hygiene", "Defects introduced - Dev/QA")
- **Resource Names**: Individual resources being tracked (e.g., "Ajay","Vivek")
- **Sprint Values**: Binary values where:
  - `SP13:Met` = Compliant/Met KPI target (green)
  - `SP14:Not Met` = Non-compliant/Missed KPI target (red)

### 3. Example JSON Data

```json
[
  {
    "Resource": "Ajay Varma <ajaykumar.s@org.com>",
    "KPI Name": "Ado Hygiene",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "Ajay Varma <ajaykumar.s@org.com>",
    "KPI Name": "Daily Burndown for Tasks",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "Ajay Varma <ajaykumar.s@org.com>",
    "KPI Name": "Defects introduced - Dev/QA",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "vivek.jain <vivek.jain@org.com>",
    "KPI Name": "Ado Hygiene",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "vivek.jain <vivek.jain@org.com>",
    "KPI Name": "Daily Burndown for Tasks",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  },
  {
    "Resource": "vivek.jain <vivek.jain@org.com>",
    "KPI Name": "Defects introduced - Dev/QA",
    "SP13": "Met",
    "SP14": "Met",
    "SP15": "Met",
    "SP16": "Met",
    "SP17": "Met",
    "count": "0"
  }
]
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
