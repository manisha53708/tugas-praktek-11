# ShopCatalog Pro - REST API Client App

A functional Mobile Application built using React Native and Expo to consume data from a Public REST API. This project showcases structured state management, error handling, client-side data manipulation, and modern UI practices.

## 📱 Features

### Level 1 — Core Features (Wajib)
- **Async/Await Integration:** Fetches product data asynchronously from FakeStore API.
- **Single Mount Fetch:** Powered by `useEffect` with an empty dependency array (`[]`).
- **3-State UI Handling:** Smooth transition states for:
  - 🔄 **Loading State:** `ActivityIndicator` display while data fetches.
  - ❌ **Error State:** Descriptive error prompt equipped with a operational **"Coba Lagi" (Retry) Button**.
  - ✅ **Success State:** Dynamic item listing using `FlatList`.
- **Advanced Error Handling:** Secured with structural `try / catch / finally` blocks ensuring proper resource disposal.
- **Robust Item Cards:** Renders standard properties including Product Image, Title, Category, and Price.

### Level 2 & 3 — Extended Features (Pilihan Tambahan)
- 🔄 **Pull-to-Refresh:** Swipe down to clear cache and reload updated data states directly from the endpoint server.
- 🔎 **Client-Side Search Filter:** Local operational searching that matches titles and categories instantly as you type.
- 📄 **Detail Modal Layout:** Tapping any product opens a safe contextual Modal containing complete metrics (Detailed description).
- 🎨 **Smart Empty State (Level 3):** Renders clean visual fallbacks instead of an empty white screen if search returns zero matches.

---

## 🛠️ Tech Stack & Tools
- **Framework:** React Native (Expo Workflow)
- **Environment Run Target:** Expo Go (Tested on Physical Device)
- **Data Source Provider:** FakeStore API (`https://fakestoreapi.com/products`)

---

## 🚀 Setup Instructions (How to Run)

Follow these steps to deploy and test the app locally on your machine:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/manisha53708/tugas-praktek-11.git](https://github.com/manisha53708/tugas-praktek-11.git)
   cd tugas-praktek-11

   | ![Loading](https://github.com/manisha53708/tugas-praktek-11/blob/main/assets/loading.jpeg) | ![Success](https://github.com/manisha53708/tugas-praktek-11/blob/main/assets/berhasil.jpeg) | ![Error](https://github.com/manisha53708/tugas-praktek-11/blob/main/assets/error.jpeg) |
