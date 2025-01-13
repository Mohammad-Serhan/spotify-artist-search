# Spotify Artist Search Application

## Overview
This project is a basic Spotify application that allows users to search for an artist and retrieve information about their albums. The app integrates with the **Spotify API** to fetch real-time data and provides a seamless user experience for music discovery.

---

## Product Specification

### A. Landing Page - Login With Spotify
1. The landing page contains a **“Login with Spotify”** button.
2. Clicking the button starts the **Spotify Implicit Grant authentication flow**.
3. Upon successful authentication, the user is redirected to the **“Artist Search”** page.

### B. Artist Search
1. The page includes a search input with placeholder text: **“Search for an artist...”**.
2. When pressing the **Return** key, the user sees the search results.
   - **Spotify artist search API**:  
     [Get Search Item](https://developer.spotify.com/console/get-search-item)
3. **Bonus**: Implements a **“search-as-you-type”** functionality.

### C. Browsing Artists
1. Displays the results from the **Artist Search**.
2. Results follow these specifications:
   - Keeps the **Spotify API ordering**.
   - Displays an **artist image**.
   - Shows the artist's **popularity** as a star rating (1-5 stars).
   - Displays the **number of followers**.
   - Results are clickable to retrieve the artist’s albums.

### D. Browsing Artist Albums
1. Displays albums for the selected artist.
   - **Spotify artist album search API**:  
     [Get Artist Albums](https://developer.spotify.com/console/get-artist-albums/)
2. Album results include:
   - **Album cover image**.
   - **Album name**.
   - **List of artists** featured on the album.
   - **Release year** of the album.
   - **Total number of tracks**.
   - A clickable link to open the **Spotify album preview** in a new tab.  
     *(Hint: Use the `external_urls` parameter from the API results.)*
3. Clicking the browser's **Back** button returns to the previous search results.


---


## Getting Started


### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/spotify-artist-search.git
   cd spotify-artist-search


### Install dependencies:
  `npm install`

## Running the Application
1. Start the development server
   `npm start`.
2. Open your browser and navigate to `http://localhost:3000`.
