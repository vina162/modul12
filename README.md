# 📍 Flutter Project - Akses Lokasi dengan GPS

A Flutter application that demonstrates how to **retrieve and display the user's current location** using the `geolocator` and `geocoding` packages.  
This project focuses on learning how to access GPS data, handle permissions, and convert coordinates into readable addresses.

## 🧩 Preview
The app displays:
- An *AppBar* titled *“Lokasi Saya”* with a deep indigo color.  
- A *Card* widget showing:
  - Kecamatan (sub-district)
  - Kota (city)
- A *button* labeled *“TAMPILKAN LOKASI SAAT INI”* to fetch the user’s live location.  
- Loading and error messages when GPS is processing or unavailable.

## 💡 Result
When you run the app, it looks like this:
```
-------------------------------------------
| Lokasi Saya                             |
|-----------------------------------------|
| [Card]                                  |
|  Kelurahan/Kecamatan: Cipedes           |
|  Kota: Tasikmalaya                      |
|-----------------------------------------|
| [ TAMPILKAN LOKASI SAAT INI ]           |
-------------------------------------------
```

If the location service is off or permission is denied, an error message will be displayed instead.

## ⚙️ Key Functionality
### 🔹 _getLocation()
Handles the entire process of:
1. Checking GPS service availability.  
2. Requesting location permission.  
3. Fetching current coordinates (latitude & longitude).  
4. Converting coordinates into readable address info (kecamatan & kota).

### 🔹 Variables:
- `_isLoading` → Controls the loading state while fetching data.  
- `_kecamatan` & `_kota` → Store the name of the user’s sub-district and city.  
- `_errorMessage` → Stores any errors related to permission or GPS access.

## 🛠️ Tech Used
- *Flutter SDK*
- *Dart Language*
- *geolocator* (to access GPS)
- *geocoding* (to translate coordinates into address)
- *Google Fonts (Poppins)* for modern typography
- *Material Design Widgets*

✨ *An elegant and educational Flutter project that shows how to integrate GPS features and real-time location data into your mobile app!*  
````
