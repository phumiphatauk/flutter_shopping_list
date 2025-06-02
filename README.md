# 🛒 Flutter Shopping List

A modern and intuitive shopping list app built with Flutter and Firebase. Organize your grocery shopping with color-coded categories and real-time synchronization!

## ✨ Features

- 🛍️ **Smart Grocery Management** - Add, view, and delete grocery items effortlessly
- 🎨 **Color-Coded Categories** - 10 distinct categories with vibrant color coding
- ☁️ **Cloud Synchronization** - Real-time data sync with Firebase Realtime Database
- 📱 **Offline-First Design** - Optimistic UI updates for smooth user experience
- 🔄 **Swipe to Delete** - Intuitive gesture-based item removal
- ✅ **Form Validation** - Smart input validation with helpful error messages
- 🌙 **Dark Theme** - Beautiful dark theme optimized for all lighting conditions
- 📱 **Cross-Platform** - Runs seamlessly on iOS, Android, Web, macOS, Windows, and Linux
- ⚡ **Loading States** - Smooth loading indicators and error handling
- 🔒 **Environment Variables** - Secure configuration management with dotenv

## 🗂️ Categories

The app supports 10 distinct categories, each with its own color:

| Category | Color | Items |
|----------|-------|-------|
| 🥬 **Vegetables** | Green | Lettuce, Carrots, Broccoli |
| 🍎 **Fruit** | Lime Green | Apples, Bananas, Oranges |
| 🥩 **Meat** | Orange | Beef, Chicken, Pork |
| 🥛 **Dairy** | Light Blue | Milk, Cheese, Yogurt |
| 🍞 **Carbs** | Blue | Bread, Rice, Pasta |
| 🍭 **Sweets** | Amber | Candy, Chocolate, Cookies |
| 🌶️ **Spices** | Yellow | Salt, Pepper, Herbs |
| 📦 **Convenience** | Purple | Frozen foods, Canned goods |
| 🧴 **Hygiene** | Dark Purple | Soap, Shampoo, Toothpaste |
| 🔧 **Other** | Cyan | Household items, Miscellaneous |

## 🚀 Getting Started

### Prerequisites

- Flutter SDK (v3.8.0 or higher)
- Dart SDK (compatible with Flutter version)
- Firebase project with Realtime Database
- A device or emulator to run the app

### 🔧 Firebase Setup

1. Create a new Firebase project at [Firebase Console](https://console.firebase.google.com/)
2. Enable Realtime Database
3. Set up database rules for read/write access
4. Copy your Firebase Realtime Database URL

### 📥 Installation

1. Clone this repository:
```bash
git clone https://github.com/phumiphatauk/flutter_shopping_list.git
```

2. Navigate to the project directory:
```bash
cd flutter_shopping_list
```

3. Install dependencies:
```bash
flutter pub get
```

4. Create a `.env` file in the root directory:
```env
FIREBASE_URL=your-firebase-project-url
```

5. Run the app:
```bash
flutter run
```

## 🎮 How to Use

### Adding Items
1. Tap the **+** button in the app bar
2. Fill in the item details:
   - **Name**: Enter the item name (1-50 characters)
   - **Quantity**: Specify how many you need (positive number)
   - **Category**: Select from the color-coded dropdown
3. Tap **Add Item** to save to your list

### Managing Items
- **View**: All items are displayed with their category colors and quantities
- **Delete**: Swipe left on any item to remove it from your list
- **Real-time Sync**: Changes are automatically synced across all your devices

### Categories
- Each item displays a colored square indicating its category
- Choose from 10 predefined categories when adding items
- Categories help organize and visually distinguish different types of items

## 📱 Supported Platforms

- ✅ Android
- ✅ iOS  
- ✅ Web
- ✅ Windows
- ✅ macOS
- ✅ Linux

## 📦 Dependencies

```yaml
dependencies:
  flutter: sdk
  cupertino_icons: ^1.0.8    # iOS-style icons
  http: ^1.4.0               # HTTP client for API calls
  flutter_dotenv: ^5.2.1     # Environment variable management

dev_dependencies:
  flutter_test: sdk
  flutter_lints: ^5.0.0      # Code quality and style linting
```

## 🏗️ Project Structure

```
lib/
├── main.dart                    # App entry point and theme configuration
├── data/
│   ├── categories.dart         # Category definitions with colors
│   └── dummy_items.dart        # Sample grocery items
├── models/
│   ├── category.dart           # Category data model
│   └── grocery_item.dart       # Grocery item data model
└── widgets/
    ├── grocery_list.dart       # Main shopping list screen
    └── new_item.dart           # Add new item form
```

## 🎨 Design Features

- **Dark Theme**: Elegant dark theme with custom color scheme
- **Color Coding**: Each category has a distinct color for easy identification
- **Material Design**: Follows Material Design 3 principles
- **Responsive Layout**: Adapts to different screen sizes
- **Loading States**: Smooth loading indicators during network operations
- **Error Handling**: User-friendly error messages and retry mechanisms

## 🔧 Technical Features

- **Firebase Integration**: Real-time database for cloud synchronization
- **HTTP Client**: Robust networking with proper error handling
- **Form Validation**: Comprehensive input validation with visual feedback
- **State Management**: Efficient state management with StatefulWidget
- **Environment Configuration**: Secure API key management with dotenv
- **Dismissible Widgets**: Intuitive swipe-to-delete functionality
- **Optimistic Updates**: Immediate UI updates with server synchronization
- **Cross-Platform**: Single codebase for multiple platforms

## 🌐 Firebase Structure

Your Firebase Realtime Database will store data in this format:

```json
{
  "shopping-list": {
    "item_id_1": {
      "name": "Milk",
      "quantity": 1,
      "category": "Dairy"
    },
    "item_id_2": {
      "name": "Bananas",
      "quantity": 5,
      "category": "Fruit"
    }
  }
}
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/phumiphatauk/flutter_shopping_list/issues).

### How to Contribute
1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🔒 Environment Variables

Create a `.env` file in your project root:

```env
FIREBASE_URL=https://your-project-default-rtdb.firebaseio.com
```

**Note**: Never commit your `.env` file to version control. It's already included in `.gitignore`.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Flutter team for the incredible framework
- Firebase team for the backend services
- Material Design for the beautiful design system
- Community contributors and testers

## 📧 Contact

Project Link: [https://github.com/phumiphatauk/flutter_shopping_list](https://github.com/phumiphatauk/flutter_shopping_list)
