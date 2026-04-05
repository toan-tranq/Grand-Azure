Project Setup and Structure

The Grand Azure Hotel Booking Application is a single-page application (SPA) built with Vue.js 3 using Vite as the build tool and Pinia for global state management. The project is structured as a clean, maintainable frontend codebase with clear separation of concerns across assets, components, routing, state stores, and page views.

1	Installation and Running
	·	Extract hotel-booking-app.zip to a local folder.                                                  
	·	Open a terminal inside hotel-booking-app/ and run: npm install
    ·   Start the development server: npm run dev         
	·   Open http://localhost:5173 in a browser.
	·	To create a production build: npm run build

2   Folder Structure

hotel-booking-app/
├── public/
│   ├── data/
│   │   └── news.json          #Local JSON for News Page
│   └── images/                # Home/About images
├── src/
│   ├── assets/                # CSS and global styles
│   │   └── main.css           # Bootstrap grid and custom styles 
│   ├── components/            # Reusable UI components
│   │   ├── Navigation.vue     # Navbar for easy navigation 
│   │   ├── RoomCard.vue       # For comparing rooms 
│   │   └── BookingForm.vue    # Form with validation 
│   ├── directives/            
│   │   └── v-focus.js         # Example custom directive
│   ├── router/
│   │   └── index.js           # Vue Router configuration 
│   ├── views/                 # Stage 1 & 2 Page Components
│   │   ├── Home.vue           
│   │   ├── News.vue           
│   │   ├── About.vue          
│   │   ├── Login.vue         
│   │   ├── Registration.vue  
│   │   └── RoomDetail.vue     # View descriptions and cost 
│   ├── App.vue                # Main Entry Component
│   └── main.js                # Mounts Vue app and uses Router
├── index.html
├── package.json               # Dependencies (Vue, Bootstrap, Vite) 
└── vite.config.js             # Vite configuration 
