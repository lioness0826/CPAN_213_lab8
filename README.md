**CPAN 213 – Cross-Platform Mobile Application Development** 
Lab 8: Building multi-screen navigation systems

The goal of this lab is to implement a professional navigation setup using:

- Stack Navigator (Home, Details, Profile)
- Tab Navigator (Home, Search, Settings)
- Parameter passing between screens
- Custom header styling
- Basic navigation actions (`navigate`, `goBack`, `setParams`)

## install dependancies
npx @react-native-community/cli init NavigationApp
cd NavigationApp 
npm install @react-navigation/native 
npm install @react-navigation/stack 
npm install @react-navigation/bottom-tabs 
npm install react-native-screens react-native-safe-area-context 
npm install react-native-gesture-handler 
npm install react-native-vector-icons


## navigation structure
NavigationContainer
└── TabNavigator
    ├── HomeTab (StackNavigator)
    │     ├── HomeScreen
    │     ├── DetailsScreen
    │     └── ProfileScreen
    │
    ├── SearchTab
    │     └── SearchScreen
    │
    └── SettingsTab
          └── SettingsScreen

## project Setup

# clone repository
git clone <your-repo-url>
cd NavigationApp

# install dependencies
npm install

## run android
npx react-native run-android


## clean cache (bash)
cd android
gradlew clean
cd ..
npx react-native start --reset-cache
