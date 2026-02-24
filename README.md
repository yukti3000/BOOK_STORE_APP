# BOOK_STORE_APP
# 📚 BookStore - User-Friendly Book Store Mobile App

A comprehensive, mobile-first bookstore application built with React, TypeScript, and Tailwind CSS. Designed specifically for the Indian market with prices in Indian Rupees (₹) and optimized for mobile devices.
https://hatch-flare-09840612.figma.site/

## ✨ Features

### Core Functionality
- **📱 Mobile-First Design**: Fully responsive interface optimized for mobile, tablet, and desktop
- **🔍 Search & Browse**: Search books by title or author with real-time filtering
- **🎯 Category Filtering**: Browse books by 8 different genres
- **⭐ Featured & Trending**: Curated book recommendations based on ratings and reviews
- **🛒 Shopping Cart**: Full cart management with quantity controls
- **❤️ Wishlist**: Save favorite books for later
- **💳 Checkout Process**: Complete checkout flow with address and payment options
- **👤 User Profile**: Manage account, view order history, and settings

### Pages & Screens

#### 1. **Home Screen**
- Hero section with call-to-action buttons
- Featured books showcase (highest rated)
- Browse by category cards with book counts
- Trending books section (most reviewed)
- All books grid with genre filters
- Mobile-optimized 2-column grid layout

#### 2. **Book Details Screen**
- High-quality book cover images
- Complete book information (title, author, genre, price)
- Star ratings and review counts
- Detailed description
- Add to Cart and Wishlist buttons
- Additional metadata (format, publisher, language)
- Mobile-responsive layout

#### 3. **Shopping Cart Screen**
- List of cart items with thumbnails
- Quantity increment/decrement controls
- Individual item removal
- Clear all cart option
- Order summary with pricing breakdown
- Free shipping indicator
- Proceed to checkout button
- Mobile-optimized compact layout

#### 4. **Checkout Screen**
- Delivery address form with validation
- Multiple payment options:
  - UPI / PhonePe / Google Pay
  - Credit/Debit Card
  - Cash on Delivery
- Order summary sidebar
- Mobile-friendly form layout
- Success notification on order placement

#### 5. **Wishlist Screen**
- Grid view of saved books
- Quick add to cart from wishlist
- Remove items from wishlist
- Empty state with call-to-action
- Mobile-optimized card layout

#### 6. **Profile Screen** (Tabbed Interface)
- **Profile Tab**: Personal information with edit capability, account statistics
- **Orders Tab**: Order history with status tracking, itemized order details
- **Wishlist Tab**: Quick access to saved books
- **Settings Tab**: Notification preferences, account actions

### Design Features
- **🎨 Reading-Friendly Color Scheme**: Warm orange/brown primary colors (#c2410c)
- **📐 Clean Layout**: Consistent spacing and typography
- **🎭 Smooth Animations**: Hover effects and transitions
- **🔔 Toast Notifications**: User feedback for actions
- **🎯 Accessibility**: Proper contrast and readable text
- **📱 Mobile Menu**: Collapsible mobile navigation with search

### Technical Features
- **React Router**: Multi-page navigation with URL-based routing
- **Context API**: State management for cart and wishlist
- **TypeScript**: Type-safe code
- **Tailwind CSS v4**: Modern utility-first styling
- **Lucide Icons**: Beautiful, consistent iconography
- **Sonner**: Toast notifications
- **Shadcn/ui Components**: Professional UI components

## 📚 Book Catalog

The app includes 8 carefully selected books across different genres:

1. **Pride and Prejudice** (Classic) - ₹299
2. **The Mystery of the Blue Train** (Mystery) - ₹249
3. **Dune** (Science Fiction) - ₹399
4. **The Notebook** (Romance) - ₹299
5. **The Name of the Wind** (Fantasy) - ₹349
6. **Atomic Habits** (Self-Help) - ₹499
7. **Gone Girl** (Thriller) - ₹299
8. **Steve Jobs** (Biography) - ₹599

All books feature real cover images from Unsplash, ratings, review counts, and detailed descriptions.

## 🎯 User Flow

### Shopping Journey
1. Browse featured/trending books or use category navigation
2. Search for specific books or authors
3. View detailed book information
4. Add books to cart or wishlist
5. Review cart and adjust quantities
6. Proceed to checkout
7. Fill in delivery address
8. Select payment method
9. Place order
10. View order confirmation in profile

### Navigation Structure
```
Root Layout (Header + Footer)
├── Home (/)
├── Book Detail (/book/:id)
├── Cart (/cart)
├── Checkout (/checkout)
├── Wishlist (/wishlist)
└── Profile (/profile)
    ├── Profile Tab
    ├── Orders Tab
    ├── Wishlist Tab
    └── Settings Tab
```

## 🎨 Design Principles

### Visual Hierarchy
- Large, readable typography
- Clear call-to-action buttons
- Prominent book covers and pricing
- Consistent spacing system

### Mobile Optimization
- Touch-friendly button sizes (min 44x44px)
- Collapsible mobile menu
- Responsive grid layouts (2 cols mobile → 4 cols desktop)
- Bottom-aligned action buttons
- Sticky header and order summary

### User Experience
- Instant feedback with toast notifications
- Loading states and animations
- Empty states with helpful messages
- Back navigation on detail pages
- Persistent cart and wishlist state

## 🛠️ Technology Stack

- **React 18** - UI library
- **TypeScript** - Type safety
- **React Router v7** - Routing
- **Tailwind CSS v4** - Styling
- **Lucide React** - Icons
- **Sonner** - Toast notifications
- **Radix UI** - Accessible UI primitives

## 📂 Project Structure

```
src/
├── app/
│   ├── components/
│   │   ├── ui/           # Reusable UI components
│   │   ├── BookCard.tsx  # Book display card
│   │   ├── Header.tsx    # Navigation header
│   │   └── Footer.tsx    # Site footer
│   ├── context/
│   │   ├── CartContext.tsx     # Shopping cart state
│   │   └── WishlistContext.tsx # Wishlist state
│   ├── data/
│   │   └── books.ts      # Book catalog data
│   ├── pages/
│   │   ├── Root.tsx      # Layout wrapper
│   │   ├── Home.tsx      # Homepage
│   │   ├── BookDetail.tsx
│   │   ├── Cart.tsx
│   │   ├── Checkout.tsx
│   │   ├── Wishlist.tsx
│   │   └── Profile.tsx
│   ├── App.tsx           # App entry point
│   └── routes.ts         # Route configuration
└── styles/
    ├── theme.css         # Design tokens
    └── fonts.css         # Font imports
```

## 🎨 Color Palette

- **Primary**: Orange-Brown (#c2410c) - Warm, book-friendly
- **Background**: Stone (#fafaf9) - Soft, reading-friendly
- **Accent**: Peach (#fed7aa) - Subtle highlights
- **Destructive**: Red (#d4183d) - Alerts and errors
- **Text**: Dark gray - High readability

## 📱 Responsive Breakpoints

- **Mobile**: < 768px (2-column grid)
- **Tablet**: 768px - 1024px (3-column grid)
- **Desktop**: > 1024px (4-column grid)

## 🚀 Future Enhancements

- User authentication and login
- Book reviews and ratings submission
- Advanced filtering (price range, publisher)
- Book recommendations based on history
- Multiple address management
- Order tracking with delivery status
- Favorites sharing via social media
- Dark mode support
- Multi-language support (Hindi, Tamil, etc.)
- Payment gateway integration

## 📄 License

This is a demo project created for educational purposes.

---

**Made with ❤️ in India** 🇮🇳
