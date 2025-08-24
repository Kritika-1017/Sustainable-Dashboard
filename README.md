# Sustainability Dashboard for Textile Company

A comprehensive, real-time sustainability monitoring dashboard designed specifically for textile manufacturing companies to track key environmental metrics, identify operational hotspots, and ensure regulatory compliance.

## 🎯 Objective

Design a sustainability dashboard for the Head of Sustainability at a textile manufacturing company to monitor key sustainability metrics — energy, water, waste, and emissions — identify problem areas, support decisions, and ensure regulatory compliance.

## 🚀 Features

### Must-Have Features ✅

#### 1. Filters & Defaults
- **Time Filters**: Today, This Week, This Month, This Year, Last 5 Years, Last 10 Years
- **Unit Filters**: All Units, Spinning Unit, Weaving Unit, Dyeing Unit, Finishing Unit, Packaging Unit
- **Department Filters**: All Departments, Spinning, Weaving, Dyeing, Finishing, Quality Control, Maintenance, Packaging
- **Machine Filters**: All Machines, Ring Spinning Frame, Open-End Spinner, Air Jet Loom, Rapier Loom, Jig Dyeing Machine, Jet Dyeing Machine, Stenter Machine, Calendering Machine
- **Shift Filters**: All Shifts, Morning Shift (6 AM - 2 PM), Afternoon Shift (2 PM - 10 PM), Night Shift (10 PM - 6 AM)
- **Default Selection**: Today + All Units + All Departments
- **Persistent State**: Filter state persists after reload

#### 2. KPI & Overall Performance Tiles
- **Energy**: Real-time consumption in kWh with trend indicators
- **Water**: Usage tracking in liters with status monitoring
- **Waste**: Generation tracking in kg with limit alerts
- **Emissions**: Carbon footprint in gCO₂ with reduction tracking
- **Overall Performance**: Comprehensive sustainability score with progress indicators
- **Color-coded Status**: On Track, Over Limit, Near Limit, Optimal
- **Click-to-Explore**: Each tile opens detailed insights page

#### 3. Click-to-Explore
- **KPI Insights Pages**: Detailed analysis for each sustainability metric
- **Overall Insights Page**: Comprehensive sustainability overview
- **Drill-down Capabilities**: Granular data analysis by unit, department, machine, or shift

#### 4. Critical Alerts, Notifications, and Updates
- **High-Priority Alerts**: Immediate visibility for critical issues
- **Severity Classification**: High, Info, Low priority levels
- **Category Grouping**: Resource Usage, Operations, Compliance
- **Real-time Updates**: Timestamp tracking and status monitoring
- **Bell Icon Access**: Quick access to all alerts and notifications

#### 5. Insights Section
- **Trend-based Insights**: Line charts showing performance over time
- **Anomaly Detection**: Red bars/heatmaps for metric deviations
- **Hotspot Identification**: Bar charts pinpointing problem areas
- **Goal Progress**: Progress bars with milestone timelines
- **Change-based Insights**: Before/after comparisons
- **Cost-impact Insights**: Financial implications of sustainability practices

#### 6. Graphs & Comparisons
- **Line Graphs**: Trends over time
- **Bar Charts**: Unit, department, or shift comparisons
- **Heatmaps**: Granular level spike identification
- **Donut/Progress Charts**: Goal tracking
- **Graph Type Toggle**: Switch between visualization types
- **Multi-year Comparisons**: 5 and 10-year historical analysis

#### 7. Goals Progress Tracker
- **Energy Efficiency Target**: 85% target with current 78% progress
- **Water Conservation Goal**: 80% target with current 82% progress
- **Waste Reduction Target**: 75% target with current 65% progress
- **Carbon Footprint Reduction**: 90% target with current 88% progress
- **Overall Sustainability Score**: 90/100 target with current 85/100
- **Status Indicators**: On Track, Behind Schedule, Completed
- **Milestone Tracking**: Quarterly targets and deadlines

#### 8. Export & Reporting
- **Multiple Formats**: PDF, CSV, Excel export options
- **Report Types**: Summary and detailed breakdowns
- **Date Range Selection**: Flexible time period selection
- **Custom Notes**: Add contextual information and insights
- **Company Branding**: Include logo, colors, and company information
- **Professional Reports**: Audit-ready documentation

#### 9. Refresh Button
- **Automatic Updates**: Metrics refresh at regular intervals
- **Manual Refresh**: On-demand data updates
- **Last Updated Timestamp**: Real-time status tracking

### Good-to-Have Features 🌟

#### 1. Sticky Notes / Comments
- **Metric Annotations**: Add notes to specific data points
- **Team Visibility**: Share insights across sustainability team
- **Historical Context**: Maintain context for future analysis

#### 2. Event Overlay on Graphs
- **Operational Events**: Mark maintenance, shutdowns, and incidents
- **Cause-and-Effect Analysis**: Understand metric spikes and dips
- **Timeline Integration**: Visual correlation with performance data

#### 3. Comparison View
- **Side-by-Side Analysis**: Compare units, departments, shifts, or time periods
- **Dual-Axis Charts**: Multi-metric comparison capabilities
- **Benchmark Analysis**: Performance against industry standards

#### 4. Action Tracker
- **Observations to Tasks**: Convert insights into trackable actions
- **Team Assignment**: Assign responsibilities to team members
- **Status Updates**: Track progress (In Progress, Resolved)
- **Follow-up Management**: Ensure timely resolution

#### 5. Auto Weekly Email Summary
- **Stakeholder Communication**: Weekly KPI summaries
- **Anomaly Reports**: Highlight critical issues
- **Progress Updates**: Goal achievement status
- **Scheduled Delivery**: Automated reporting

#### 6. AI-Based Recommendations
- **Operational Improvements**: AI-suggested optimizations
- **Pattern Detection**: Identify efficiency opportunities
- **Predictive Analytics**: Forecast potential issues
- **Best Practice Suggestions**: Industry-standard recommendations

#### 7. Custom Alerts / Rules
- **Personalized Thresholds**: User-defined alert levels
- **Scheduled Notifications**: Proactive monitoring setup
- **Conditional Alerts**: Complex rule-based notifications
- **Escalation Paths**: Multi-level alert routing

#### 8. Audit Logs
- **Data Updates**: Track all metric changes
- **User Actions**: Monitor dashboard interactions
- **Transparency**: Support regulatory audits
- **Compliance**: Maintain audit trail

## 🛠️ Technology Stack

- **Frontend**: React 18 with TypeScript
- **Styling**: Tailwind CSS with custom design system
- **Charts**: Recharts for data visualization
- **Icons**: Lucide React for consistent iconography
- **Build Tool**: Vite for fast development and building
- **State Management**: React Context API for filters and state
- **Responsive Design**: Mobile-first approach with breakpoint optimization

## 📱 Responsive Design

- **Mobile-First**: Optimized for shop floor and mobile devices
- **Breakpoint System**: 
  - `sm`: 640px+ (Small tablets)
  - `md`: 768px+ (Tablets)
  - `lg`: 1024px+ (Laptops)
  - `xl`: 1280px+ (Desktops)
- **Touch-Friendly**: Optimized for touch interactions
- **Flexible Layouts**: Adaptive grid systems for different screen sizes

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd sustainability-dashboard
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open in browser**
   Navigate to `http://localhost:5173`

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## 📁 Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── charts/         # Chart components (Trend, Hotspot, Comparison, etc.)
│   ├── AlertsPanel.tsx # Critical alerts and notifications
│   ├── ExportModal.tsx # Export and reporting functionality
│   ├── FiltersBar.tsx  # Data filtering controls
│   ├── GoalsSection.tsx # Sustainability goals tracking
│   ├── Header.tsx      # Main navigation and branding
│   ├── MetricCard.tsx  # Individual KPI display cards
│   ├── MetricsGrid.tsx # KPI grid layout
│   └── RecentActivity.tsx # Recent sustainability activities
├── context/            # React context providers
│   └── FiltersContext.tsx # Filter state management
├── pages/              # Page components
│   └── InsightsPage.tsx # Detailed metric insights
├── services/           # Data services and API calls
│   └── sustainabilityData.ts # Mock data service
├── App.tsx            # Main application component
├── main.tsx           # Application entry point
└── index.css          # Global styles and Tailwind imports
```

## 🎨 Design System

### Color Palette
- **Primary**: Emerald (#10b981) - Sustainability focus
- **Secondary**: Blue (#3b82f6) - Energy and water
- **Accent**: Purple (#8b5cf6) - Waste management
- **Warning**: Amber (#f59e0b) - Near limits
- **Danger**: Red (#ef4444) - Over limits
- **Success**: Green (#22c55e) - On track

### Typography
- **Headings**: Inter font family with bold weights
- **Body**: System font stack for optimal readability
- **Monospace**: For data values and technical information

### Components
- **Cards**: Rounded corners with subtle shadows
- **Buttons**: Consistent hover states and transitions
- **Forms**: Accessible input styling with focus states
- **Charts**: Clean, minimal design with clear data visualization

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the project root:

```env
VITE_API_BASE_URL=your_api_endpoint
VITE_COMPANY_NAME=Your Company Name
VITE_DASHBOARD_TITLE=Sustainability Dashboard
```

### Customization
- **Company Branding**: Update company name and logo in Header component
- **Metrics**: Modify KPI definitions in MetricsGrid component
- **Goals**: Adjust sustainability targets in GoalsSection component
- **Filters**: Customize filter options in FiltersContext

## 📊 Data Integration

### Current Implementation
- **Mock Data Service**: `sustainabilityData.ts` provides sample data
- **Real-time Updates**: Simulated with refresh functionality
- **Filter Persistence**: Local storage for user preferences

### Production Integration
- **API Endpoints**: Replace mock service with real API calls
- **WebSocket**: Real-time data streaming for live updates
- **Database**: Connect to your sustainability data warehouse
- **Authentication**: Implement user authentication and role-based access

## 🧪 Testing

### Run Tests
```bash
npm run test
```

### Test Coverage
```bash
npm run test:coverage
```

## 📈 Performance Optimization

- **Lazy Loading**: Components load on demand
- **Memoization**: React.memo for expensive components
- **Bundle Splitting**: Code splitting for better load times
- **Image Optimization**: Optimized chart rendering

## 🔒 Security Considerations

- **Input Validation**: Sanitize all user inputs
- **XSS Prevention**: Secure rendering of dynamic content
- **CSRF Protection**: Implement CSRF tokens for form submissions
- **Data Encryption**: Encrypt sensitive sustainability data

## 📋 Browser Support

- **Modern Browsers**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
- **Mobile Browsers**: iOS Safari 14+, Chrome Mobile 90+
- **Progressive Enhancement**: Core functionality works without JavaScript

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:
- **Documentation**: Check this README and inline code comments
- **Issues**: Create an issue in the repository
- **Contact**: Reach out to the development team

## 🎯 Success Metrics

The dashboard implementation will be measured by:

1. **Reduction in Reporting Time**: Faster sustainability report generation
2. **Resource Efficiency**: 15%+ reduction in energy, water, waste, and emissions
3. **Alert-to-Action Time**: Reduced from 1 day to under 2 hours
4. **Regulatory Compliance**: 100% audit readiness
5. **Stakeholder Transparency**: Improved management and board confidence
6. **Data Accessibility**: Centralized, user-friendly data access
7. **Goal Achievement**: Higher rate of meeting sustainability targets

## 🔮 Future Enhancements

- **Machine Learning**: Predictive analytics for sustainability trends
- **IoT Integration**: Real-time sensor data from manufacturing equipment
- **Blockchain**: Immutable sustainability data tracking
- **Mobile App**: Native mobile application for field workers
- **API Ecosystem**: Third-party integrations and data sharing
- **Advanced Analytics**: Statistical analysis and correlation studies

---

**Built with ❤️ for sustainable textile manufacturing**

*Last updated: December 2024*
