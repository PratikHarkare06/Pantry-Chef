# Pantry Chef - Recipe Generator App

## Overview

Pantry Chef is a fully functional web application that helps users generate recipes based on ingredients they have in their kitchen. The app provides an intuitive interface for ingredient management, recipe discovery, and saved recipes tracking.

## Features Implemented

### 1. **Ingredient Management**

- ✅ Add ingredients manually via text input
- ✅ Remove individual ingredients
- ✅ Clear all ingredients at once
- ✅ Display ingredient count
- ✅ Ingredient icons and color coding by category
- ✅ Scan receipt (simulated) to add multiple ingredients
- ✅ AI Vision (simulated) to detect ingredients from images
- ✅ Persistent storage with localStorage

### 2. **Staples & Preferences**

- ✅ Toggle common staples (Olive Oil, Salt, Pepper, Butter, Milk)
- ✅ Visual selection indicators
- ✅ Dietary preferences selection (Vegetarian, Gluten-Free, Dairy-Free, Nut-Free, Low Carb)
- ✅ Cooking skill level selection (Novice or Pro)

### 3. **Recipe Generation**

- ✅ Intelligent recipe generation based on available ingredients
- ✅ Dynamic recipe matching (shows match percentage)
- ✅ Includes prep time, cook time, ingredients list, and step-by-step instructions
- ✅ Multiple recipe suggestions based on ingredient combinations:
  - Golden Potato Hash (for eggs + potatoes)
  - Cheesy Spinach Bake (for spinach + cheese)
  - Pantry Surprise (fallback recipe using any ingredients)

### 4. **Recipe Discovery**

- ✅ View suggested recipes based on ingredients
- ✅ Recipe cards with images, ratings, difficulty level, and cook time
- ✅ Click recipe cards to view detailed information
- ✅ Pantry match score visualization
- ✅ Filter recipes by ingredients used

### 5. **Recipe Details View**

- ✅ Full recipe display with hero image
- ✅ Prep and cook time display
- ✅ Complete ingredients list with color coding
- ✅ Step-by-step cooking instructions
- ✅ Add to/remove from favorites (heart icon)
- ✅ "I Cooked This!" action to track cooked recipes

### 6. **Saved Recipes**

- ✅ View all saved/favorited recipes
- ✅ Recipe filtering by category
- ✅ Display cooking statistics:
  - Recipes cooked
  - Recipes saved
  - Average rating
- ✅ Quick access to add more ingredients via "Add Milk" suggestion

### 7. **Chef Profile**

- ✅ User profile display with avatar
- ✅ Chef stats (recipes created, meals cooked, XP points)
- ✅ Dietary preferences display
- ✅ Cooking skill level selection
- ✅ Weekly nutrition chart
- ✅ About me section

### 8. **User Settings**

- ✅ Dark mode toggle with persistence
- ✅ Profile editing capabilities
- ✅ Settings button access

### 9. **Navigation**

- ✅ Five main views:
  1.  Ingredients (home/main screen)
  2.  Discovery (recipe suggestions)
  3.  Recipe Detail (full recipe view)
  4.  Saved Recipes (favorites)
  5.  Chef Profile (user settings)
- ✅ Smooth navigation with back buttons
- ✅ Toast notifications for user feedback

### 10. **Data Persistence**

- ✅ localStorage integration for all user data:
  - Ingredients list
  - Staples preferences
  - Dietary preferences
  - Cooking skill level
  - Saved recipes
  - Dark mode preference

## Technical Stack

- **HTML5** - Semantic markup with Material Design icons
- **CSS3** - Modern styling with CSS variables for theming and dark mode support
- **Vanilla JavaScript** - No frameworks, pure DOM manipulation
- **Material Symbols Rounded icons** - Google's icon library
- **Google Fonts** - Plus Jakarta Sans and Nunito fonts

## Browser Compatibility

- Modern browsers (Chrome, Firefox, Safari, Edge)
- HTML5 and CSS3 support required
- localStorage support required for data persistence

## How to Use

### Adding Ingredients

1. Type an ingredient name in the input field
2. Press Enter or click the Add button
3. The ingredient appears in the list below

### Generating a Recipe

1. Add at least one ingredient
2. Click "Generate Magic Recipe" button
3. View the generated recipe with details

### Saving a Recipe

1. Open a recipe detail view
2. Click the heart icon to favorite/save
3. Access saved recipes from the "Saved Recipes" view

### Profile Customization

1. Click your avatar in the top right
2. Select dietary preferences and skill level
3. Toggle dark mode in settings
4. Click "Save Profile Changes"

## File Structure

```
Recipie Generator/
├── index.html              # Main HTML file with all views
├── app.js                  # JavaScript application logic (694 lines)
├── styles.css              # Complete styling (889 lines)
└── README.md              # This file
```

## Notable Functions (in app.js)

- `addIngredient()` - Add ingredient to list
- `removeIngredient(index)` - Remove ingredient
- `toggleStaple(index)` - Toggle staple ingredient
- `generateRecipe()` - Create recipe from ingredients
- `renderIngredients()` - Update ingredient display
- `renderRecipeCards()` - Display recipe list
- `showView(view)` - Navigation between screens
- `showToast(message)` - Display notifications

## Recent Fixes

- ✅ Added missing `removeIngredient()` function
- ✅ Added missing `toggleStaple()` function
- ✅ Fixed navigation calls to use `showView()` instead of undefined `navigateToView()`
- ✅ Consolidated event listeners for cleaner code
- ✅ All DOM elements reference correct IDs
- ✅ All functions properly defined and connected

## Deployment

To use locally:

1. Open `index.html` in a web browser, or
2. Start a local server: `python3 -m http.server 8000`
3. Navigate to `http://localhost:8000`

All data is stored in the browser's localStorage, so recipes and preferences persist between sessions.

---

**App Version:** 1.0 (Fully Functional)
**Last Updated:** March 30, 2026
