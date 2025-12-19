# Closet Sensei 👔✨

Closet Sensei leverages deep learning to analyze your clothing items and generate intelligent outfit recommendations based on style compatibility, occasion, weather, and personal preferences. Built with React Native for seamless cross-platform experience and powered by ResNet50 for accurate clothing classification.

## ✨ Features

- **Smart Wardrobe Management**: Upload and categorize your clothing items with AI assistance
- **Intelligent Outfit Generation**: Get personalized outfit recommendations using ResNet50-powered analysis
- **Style Matching**: Advanced algorithms ensure color coordination and style compatibility
- **Occasion-Based Suggestions**: Receive outfit recommendations tailored to specific events or settings
- **Weather Integration**: Get weather-appropriate outfit suggestions
- **Favorites & History**: Save your favorite combinations and track outfit usage
- **Cross-Platform**: Available on both iOS and Android

## 🏗️ Architecture

### Frontend
- **React Native**: Cross-platform mobile application
- **Expo**: Development and build tooling
- **React Navigation**: Seamless navigation experience

### Backend & AI
- **AWS Lambda**: Serverless compute for outfit generation logic
- **Amazon S3**: Scalable storage for clothing images
- **AWS API Gateway**: RESTful API endpoints
- **ResNet50**: Deep learning model for clothing classification and feature extraction
- **Python**: Backend processing and ML inference

### Infrastructure
- **AWS CloudFront**: Global CDN for fast image delivery
- **AWS Certificate Manager**: SSL/TLS certificates
- **Amazon DynamoDB**: User data and outfit history storage

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- Expo CLI: `npm install -g expo-cli`
- AWS Account (for backend deployment)
- Python 3.8+ (for ML model development)

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/closet-sensei.git
cd closet-sensei
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
```bash
cp .env.example .env
```

Add your configuration:
```env
AWS_REGION=us-east-1
AWS_S3_BUCKET=your-bucket-name
API_GATEWAY_URL=your-api-url
```

4. Start the development server
```bash
expo start
```

### Running the App

- **iOS Simulator**: Press `i` in the terminal
- **Android Emulator**: Press `a` in the terminal
- **Physical Device**: Scan the QR code with Expo Go app

## 🤖 ML Model Details

### ResNet50 Implementation

The outfit recommendation system uses a fine-tuned ResNet50 model for:
- **Clothing Classification**: Identifying garment types (shirts, pants, shoes, etc.)
- **Feature Extraction**: Generating embeddings for style similarity matching
- **Color Analysis**: Extracting dominant colors and patterns

## 🛠️ Tech Stack

**Frontend:**
- React Native
- Expo
- TypeScript
- React Navigation
- Axios

**Backend:**
- Python
- OpenCV/PyTorch
- AWS Lambda
- boto3

**Infrastructure:**
- Amazon S3
- AWS CloudFront
- AWS API Gateway
- Amazon DynamoDB
- AWS Lambda

## 📱 Key Screens

1. **Wardrobe**: Browse and manage your clothing collection
2. **Outfit Generator**: Get AI-powered outfit suggestions
3. **Calendar**: Plan outfits for upcoming events
4. **Analytics**: Track your wardrobe usage and style insights
5. **Profile**: Customize preferences and style settings

## 🔐 Security & Privacy

- All images encrypted at rest in S3
- HTTPS-only communication via CloudFront
- User data stored securely in DynamoDB
- No third-party data sharing
- Local image processing option available

## 🚧 Roadmap

- [x] Social features: Share outfits with friends
- [x] Virtual try-on using AR
- [x] Integration with online shopping platforms
- [x] Seasonal wardrobe analytics
- [x] Sustainability score for outfits
- [x] Style inspiration feed

## 👨‍💻 Mentees

- **Keane:** Worked on AWS Bedrock Agent workflow
- **Jiya**: Designed and implemented the DynamoDB database schemas for different data types
- **Shreyas:** Researched various API providers for weather data and implemented caching with Redis
- **Daniel:** Implemented the Resnet model and pre-processed the clothing data using OpenCV
- **Munnawaar:** Created the prototype of the Closet Sensei app on Figma and implemented it using React Native 
