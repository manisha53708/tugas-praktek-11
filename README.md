# 📱 ShopCatalog Pro - REST API Client Application

A robust Mobile Application built using **React Native** and the **Expo Workflow** designed to consume, filter, and present data dynamically from a public REST API endpoint. This project serves as a comprehensive implementation of modern mobile development standards, showcasing structured state management, graceful error handling, and intuitive client-side interactions.

---

## 🎯 Project Assignment Overview

- **Timeframe / Deadline:** 1 Week
- **Core Technology Stack:** React Native (Expo Go Framework)
- **Data Architecture:** REST API Integration via `fetch` utilizing modern asynchronous JavaScript (`async/await`).
- **Target Endpoint:** FakeStore API (`https://fakestoreapi.com/products`)

---

## 📱 Implemented Features & Rubric Checklist

### 🟢 Level 1 — Core Features (100% Compliant)
- **Asynchronous Data Layer:** Fully integrated API requests using standard `fetch` with `async/await` syntax wrapped securely inside a lifecycle `useEffect` hook to prevent memory leaks and infinite rendering loops.
- **Robust 3-State UI System:**
  - 🔄 **Loading State:** Native `ActivityIndicator` displays a clean loader during background data fetching.
  - ❌ **Error State:** Implements custom catch-blocks that render helpful messages along with a fully operational **"Coba Lagi" (Retry) Button** that re-triggers the lifecycle fetch function.
  - ✅ **Success State:** Seamlessly lists raw catalog data once the payload successfully transfers from the server.
- **Defensive Error Handling:** Code block architecture structured around strict `try / catch / finally` handling where active loaders are systematically killed inside the `finally` block regardless of completion status.
- **Optimized List Rendering:** Implements the `FlatList` component equipped with proper unique `keyExtractor` indexing.
- **Rich Context Cards:** Each visual card displays a minimum of three required data fields: Product Image, Product Title, Category Tag, and Price Currency.

### 🟡 Level 2 — Advanced Enhancements (Selected Features)
- 🔄 **Pull-to-Refresh:** Screen-swipe gesture trigger bound directly to the `refreshControl` prop, allowing users to forcefully wipe cache states and reload original listings from the endpoint.
- 🔎 **Client-Side Search Filter:** Live interactive text monitoring input (`TextInput`) that processes and dynamically reduces the native list layout by scanning product titles or categories instantly on the user's physical hardware.
- 📄 **Detail Modal Display Overlay:** Tapping any product card halts core viewport focus to cleanly slide up a contextual, high-fidelity native `Modal` sheet carrying extensive parameters including deep descriptions.

### 🔴 Level 3 — Bonus Integration (+ Extra Grade Points)
- 🎨 **Smart UI Empty State:** Introduces a custom fallback view layout (`ListEmptyComponent`) that populates the viewport with diagnostic feedback alerts if a client-side search query yields zero items.

---

## 📸 Screenshots (Expo Go Test Cases)

Below are the verified test case representations conducted on a physical mobile hardware layer via the **Expo Go** environment:

| 🔄 1. Loading State | ✅ 2. Success State | ❌ 3. Error State (+ Retry) |
| :---: | :---: | :---: |
| ![Loading](https://github.com/manisha53708/tugas-praktek-11/blob/main/assets/loading.jpeg) | ![Success](https://github.com/manisha53708/tugas-praktek-11/blob/main/assets/berhasil.jpeg) | ![Error](https://github.com/manisha53708/tugas-praktek-11/blob/main/assets/error.jpeg) |

---

## 🚀 Setup & Execution Instructions

Follow these instructions to clone, boot, and test the system locally on your environment terminal:

### 1. Clone the Source Repository
```bash
git clone [https://github.com/manisha53708/tugas-praktek-11.git](https://github.com/manisha53708/tugas-praktek-11.git)
cd tugas-praktek-11
