<div align="center">

# 🚁 Intelligent Delivery Drone Planner

### Advanced Route Optimization with Machine Learning & Weather Intelligence

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

*Optimize drone delivery routes using Perceptron classification and Simulated Annealing algorithms*

[🚀 Live Demo](https://your-hosting-url.com) • [📊 Sample Dataset](weather_data_linearly_separable.xlsx) • [📖 Documentation](#documentation)

</div>

---

## 🌟 Overview

The **Intelligent Delivery Drone Planner** is a sophisticated web-based application that combines machine learning and optimization algorithms to solve real-world drone delivery challenges. The system uses a Perceptron classifier to predict weather safety conditions and Simulated Annealing to find the most cost-effective delivery routes while avoiding dangerous weather zones.

### 🎯 Key Objectives
- **Weather Safety Prediction**: Use Perceptron classification to identify safe flying conditions
- **Route Optimization**: Apply Simulated Annealing to minimize delivery costs
- **Cost-Aware Planning**: Integrate weather penalties into route calculations
- **Interactive Visualization**: Provide real-time visual feedback of optimization process

## 🌟 Key Features

### 🤖 Machine Learning Integration
- **Perceptron Classifier**: Binary classification for weather safety prediction
- **Real-time Training**: Train models on custom or sample datasets
- **Feature Analysis**: Process temperature, humidity, and wind speed data
- **Classification Accuracy**: Display model performance metrics

### 🛣️ Route Optimization
- **Simulated Annealing**: Advanced metaheuristic optimization algorithm
- **Dynamic Cost Calculation**: Euclidean distance + weather penalty system
- **Parameter Tuning**: Adjustable temperature, cooling rate, and penalty values
- **Route Comparison**: Before/after optimization visualization

### 📊 Interactive Dashboard
- **Drag & Drop Upload**: Excel (.xlsx, .xls) and CSV file support
- **Real-time Visualization**: 2D route mapping with SVG graphics
- **City Management**: Add, edit, and configure delivery locations
- **Weather Classification**: Visual indicators for safe/unsafe conditions

### 🎨 User Experience
- **Responsive Design**: Works seamlessly across all devices
- **Modern UI**: Clean, professional interface with smooth animations
- **Interactive Controls**: Click-to-edit city parameters
- **Progress Feedback**: Real-time optimization status updates

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No installation required - runs entirely in browser

### Getting Started

1️⃣ **Access the Application**
```
Open the HTML file in your web browser or visit the live demo
```

2️⃣ **Upload Weather Data**
- Use the provided sample dataset or upload your own
- Supported formats: Excel (.xlsx, .xls) and CSV files
- Required columns: Temperature, Humidity, Wind Speed, SafeToFly

3️⃣ **Configure Cities**
- Generate random cities or manually set coordinates
- Adjust weather parameters for each location
- Customize the number of delivery points (3-15 cities)

4️⃣ **Train & Optimize**
```bash
Train Perceptron → Classify Weather → Optimize Route
```

## 📁 Project Structure

```
intelligent-delivery-drone-planner/
├── index.html              # Main application file
├── README.md               # Project documentation
├── weather_data_linearly_separable.xlsx  # Sample dataset
└── assets/
    └── drone.jpg           # Background image (optional)
```

## 🛠️ Built With

### Core Technologies
- 🌐 **HTML5**: Structure and semantic markup
- 🎨 **CSS3**: Modern styling with animations and gradients
- ⚡ **JavaScript (ES6+)**: Application logic and algorithms
- 🎯 **TailwindCSS**: Utility-first CSS framework

### External Libraries
- 📊 **PapaParse**: CSV parsing and processing
- 📈 **SheetJS**: Excel file reading and manipulation
- 🎨 **SVG**: Vector graphics for route visualization

### Algorithms Implemented
- 🧠 **Perceptron Classifier**: Binary classification algorithm
- 🔥 **Simulated Annealing**: Metaheuristic optimization
- 📐 **Euclidean Distance**: Geographic distance calculation

## 📊 Core Features

### Machine Learning Pipeline
```
Data Upload → Preprocessing → Perceptron Training → Weather Classification
```

### Optimization Process
```
Random Route → Cost Calculation → Simulated Annealing → Optimized Route
```

### Cost Function
```
Total Cost = Σ(Distance + Weather Penalty)
Weather Penalty = Unsafe City × Penalty Factor
```

## 🎯 Algorithm Details

### Perceptron Classifier
- **Learning Rate**: 0.001 (adjustable)
- **Epochs**: 5000 maximum iterations
- **Activation Function**: Step function (threshold-based)
- **Features**: Temperature, Humidity, Wind Speed
- **Output**: Binary classification (0: Safe, 1: Unsafe)

### Simulated Annealing
- **Initial Temperature**: 1000 (configurable)
- **Cooling Rate**: 0.995 (adjustable)
- **Neighborhood**: 2-opt swap operation
- **Acceptance Probability**: Exponential decay function
- **Termination**: Temperature threshold or convergence

## 📈 Dataset Requirements

### Input Format
| Column | Data Type | Description |
|--------|-----------|-------------|
| Temperature | Float | Temperature in Celsius (°C) |
| Humidity | Float | Relative humidity percentage (%) |
| Wind Speed | Float | Wind speed in km/h |
| SafeToFly | Integer | Binary label (0: Safe, 1: Unsafe) |

### Sample Data Structure
```csv
Temperature,Humidity,WindSpeed,SafeToFly
15.5,45.2,8.3,0
32.1,78.9,25.4,1
```

## 🎮 Usage Guide

### Step 1: Dataset Preparation
1. Upload your weather dataset or use the sample data
2. Ensure proper column naming and data types
3. Verify data quality in the preview panel

### Step 2: Model Training
1. Click "Train Perceptron" to start machine learning process
2. Monitor training accuracy in the results panel
3. Review model performance metrics

### Step 3: City Configuration
1. Generate random cities or manually configure locations
2. Set weather parameters for each delivery point
3. Adjust the number of cities as needed

### Step 4: Weather Classification
1. Apply trained model to classify city weather conditions
2. Review safe/unsafe predictions for each location
3. Observe color-coded visualization updates

### Step 5: Route Optimization
1. Configure Simulated Annealing parameters
2. Run optimization algorithm
3. Compare initial vs. optimized routes
4. Analyze cost improvements and performance gains

## ⚙️ Configuration Options

### Simulated Annealing Parameters
- **Initial Temperature**: Controls algorithm exploration (default: 1000)
- **Cooling Rate**: Convergence speed (default: 0.995)
- **Unsafe Penalty**: Cost increase for dangerous locations (default: 50)

### Perceptron Settings
- **Learning Rate**: Weight adjustment magnitude (default: 0.001)
- **Max Epochs**: Training iteration limit (default: 5000)

### City Configuration
- **Number of Cities**: Delivery locations count (3-15)
- **Coordinate Range**: X: 50-550, Y: 50-350
- **Weather Ranges**: Realistic temperature, humidity, and wind values

## 📊 Performance Metrics

### Classification Metrics
- **Accuracy**: Percentage of correct weather predictions
- **Training Time**: Model convergence duration
- **Feature Importance**: Impact of weather parameters

### Optimization Metrics
- **Cost Reduction**: Percentage improvement in route cost
- **Distance Optimization**: Pure distance vs. weather-aware optimization
- **Convergence Rate**: Algorithm efficiency and speed

## 🎨 Visual Features

### Route Visualization
- **Initial Route**: Red dashed lines showing random path
- **Optimized Route**: Green solid lines displaying improved route
- **City Markers**: Color-coded circles (green: safe, red: unsafe)
- **Interactive Elements**: Click-to-edit functionality

### User Interface
- **Modern Design**: Clean, professional appearance
- **Responsive Layout**: Adapts to different screen sizes
- **Real-time Updates**: Dynamic content refresh
- **Progress Indicators**: Visual feedback for long operations

## 🔬 Technical Implementation

### Perceptron Algorithm
```javascript
class Perceptron {
    constructor(learningRate = 0.001, epochs = 5000) {
        this.learningRate = learningRate;
        this.epochs = epochs;
        this.weights = null;
        this.bias = 0;
    }
    
    train(trainingData) {
        // Initialize weights randomly
        // Iterate through epochs
        // Update weights based on prediction errors
        // Apply gradient descent optimization
    }
}
```

### Simulated Annealing Implementation
```javascript
function simulatedAnnealing(initialRoute, initialTemp, coolingRate) {
    // Initialize current and best solutions
    // Temperature-based acceptance probability
    // 2-opt neighborhood exploration
    // Exponential cooling schedule
    // Return optimized route
}
```

## 🚨 Error Handling

### Data Validation
- **File Format**: Automatic detection of Excel/CSV formats
- **Column Validation**: Ensures required columns are present
- **Data Type Checking**: Validates numeric values and ranges
- **Missing Data**: Handles incomplete records gracefully

### User Input Validation
- **Parameter Bounds**: Enforces valid ranges for all inputs
- **City Coordinates**: Prevents overlapping or invalid positions
- **Weather Values**: Realistic ranges for meteorological data

## 🔍 Troubleshooting

### Common Issues
1. **File Upload Problems**: Ensure file format is supported (.xlsx, .xls, .csv)
2. **Training Failures**: Check dataset quality and column names
3. **Optimization Errors**: Verify cities are generated and classified
4. **Performance Issues**: Reduce number of cities or epochs for slower devices

### Data Format Requirements
- Use standard column names or similar variations
- Ensure numeric data types for all features
- Binary classification labels (0/1) for SafeToFly column

## 🤝 Contributing

We welcome contributions to improve the Intelligent Delivery Drone Planner! Here's how you can help:

1. **Fork the Repository**
2. **Create a Feature Branch** (`feature/amazing-improvement`)
3. **Implement Your Changes**
4. **Test Thoroughly**
5. **Submit a Pull Request**

### Areas for Contribution
- Additional optimization algorithms (Genetic Algorithm, Ant Colony)
- Enhanced machine learning models (SVM, Neural Networks)
- Advanced visualization features
- Mobile responsiveness improvements
- Performance optimizations

## 📚 Educational Value

### Learning Outcomes
- **Machine Learning**: Understand Perceptron classification principles
- **Optimization**: Learn metaheuristic algorithm implementation
- **Algorithm Integration**: Combine multiple algorithms for complex problems
- **Web Development**: Modern JavaScript and CSS techniques
- **Data Processing**: File parsing and manipulation skills

### Suitable For
- Computer Science students
- Machine Learning enthusiasts
- Operations Research practitioners
- Web Development learners
- Algorithm implementation practice


<div align="center">

### 🌟 Star this project if you find it useful!

**Made with ❤️ for the AI and optimization community**

[⬆ Back to Top](#-intelligent-delivery-drone-planner)

</div>
