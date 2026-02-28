# Forms - Craft Management Application

## Project Description

A web-based form application for managing craft projects. This application allows users to add, track, and estimate craft projects with detailed information about timelines, costs, and technical specifications.

## Features

- **Craft Information Entry**: Add craft code, name, category, and location
- **Work Category Selection**: Choose from Woodwork, Metalwork, Textiles, or Ceramics
- **Production Type**: Select between Handmade or Machine-made options
- **Timeline Management**: Set estimated start and end dates
- **Material Type**: Select from various materials (Wood, Metal, Fabric, Clay, Glass, Composite)
- **Budget Tracking**: Set project budget amount
- **Cost Estimation**: Calculate total project cost based on hourly rates
  - Automatic calculation of total days
  - Configurable hours per day
  - Customizable cost per hour
- **Status Tracking**: Track project progress (Not Started, In Progress, Completed)
- **Technical Details**: Document technical specifications and descriptions
- **Drawing References**: Include reference images
- **Item Association**: Search and associate items with the project
- **Summary View**: Display comprehensive project summary

## Project Structure

```
Forms/
├── index.html          # Main form for adding craft projects
├── summary.html        # Summary page displaying project details
├── style.css           # Styling for the HTML pages
├── images/             # Directory for reference images
│   └── drawing-reference.jpg
└── README.md           # Project documentation
```

## How to Use

1. **Open the Form**: Open `index.html` in a web browser
2. **Fill in Project Details**:
   - Enter craft code (numeric)
   - Enter craft name
   - Select work category
   - Choose production type (Handmade/Machine-made)
   - Enter location
   - Set estimated start and end dates
   - Select project status
3. **Set Cost Parameters**:
   - Define hours per day (default: 8)
   - Set cost per hour (default: $50)
   - View automatic cost calculations
4. **Add Technical Information**:
   - Include technical details
   - Add project description
   - View drawing reference
5. **Associate Items**: Search and connect items to the project
6. **Submit**: Click submit to proceed to the summary page

## Technical Details

- **Form Handling**: HTML form with GET method parameters
- **Calculations**: Real-time cost and duration calculations using JavaScript
- **Styling**: Custom CSS with color-coded sections (green, cyan, pink headers)
- **Responsive Design**: Grid-based layout with centered form presentation
- **Image Support**: Embedded drawing references for project visualization

## Browser Compatibility

Works with modern web browsers that support:
- HTML5 form elements
- JavaScript for dynamic calculations
- CSS Grid and styling

## Notes

- All form fields are required before submission
- Dates must have end date after or equal to start date
- Cost calculations update automatically when hours or rate changes
- Form data is passed via URL parameters to the summary page