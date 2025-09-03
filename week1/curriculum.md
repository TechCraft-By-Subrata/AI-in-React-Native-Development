
# 📚 Week 1 – AI & React Native Foundations (Beginner-Friendly)

---

## **1. AI vs ML vs DL vs GenAI (Why They Matter for Mobile Apps)**

* **Introduction to AI**

  * What is Artificial Intelligence? (machines mimicking human intelligence)
  * Everyday examples: Google Maps, Siri, Face Unlock.

* **Machine Learning (ML)**

  * What is ML? (systems learn from data instead of rules).
  * Example: Predicting whether an email is spam or not.
  * Types of ML: Supervised vs Unsupervised vs Reinforcement Learning.

* **Deep Learning (DL)**

  * Neural networks basics (how layers of neurons learn).
  * Example: Identifying a cat vs dog in a photo.

* **Generative AI (GenAI)**

  * What is Generative AI? (AI that creates new content: text, images, audio).
  * Example: ChatGPT (text), DALL·E (images).

* **Why They Matter for Mobile Apps**

  * AI-powered chatbots inside RN apps.
  * Voice assistants and real-time translation.
  * Image recognition apps (health, shopping, AR).
  * Personalization (recommendations, smart notifications).

---

## **2. React Native Setup Refresher (Expo + CLI)**

* **Why React Native for AI apps** (cross-platform, fast prototyping, large ecosystem).
* **Two ways of running RN apps**:

  * **Expo CLI**: beginner-friendly, managed workflow.
  * **React Native CLI**: more flexibility, native modules support.
* **Installing and running your first app**:

  * Install Node.js and npm.
  * Install Expo CLI (`npm install -g expo-cli`).
  * Create first app: `npx create-expo-app ai-notes`.
  * Run on device/emulator: `npx expo start`.
* **Folder structure refresher**:

  * `App.js` – entry file.
  * `components/` – UI components.
  * `api/` – API helper files (for later use).

---

## **3. Working with APIs (fetch, axios)**

* **What is an API?** (bridge between frontend & backend).
* **REST basics**: endpoints, GET, POST, PUT, DELETE.
* **Using fetch in React Native**:

  * Making a GET request.
  * Making a POST request with JSON body.
  * Handling errors and responses.
* **Using axios (simpler alternative)**:

  * Installing axios (`npm install axios`).
  * Example: Fetching data from a public API.
* **Best practices**:

  * Always handle errors (`try/catch`).
  * Show loading indicators (`useState` + ActivityIndicator).
  * Keep API calls in a separate `api.js` file.

---

## **4. Integrating Python/AI Backends (FastAPI / Flask)**

* **Why Python for AI backends?**

  * Rich ML libraries (scikit-learn, TensorFlow, PyTorch).
  * Easy to deploy with FastAPI/Flask.

* **Flask Basics**

  * Install Flask (`pip install flask`).
  * Create a simple API route (`/predict`).
  * Return dummy data as JSON.

* **FastAPI Basics**

  * Install FastAPI + uvicorn (`pip install fastapi uvicorn`).
  * Define a route (`/predict`) with request body + response.
  * Run server (`uvicorn main:app --reload`).
  * Test API in browser or Postman.

* **Connecting RN App with Backend**

  * Use axios/fetch to call Flask/FastAPI endpoint.
  * Display API response inside RN app (e.g., text message).

---

## **5. Week 1 Project: Notes Classifier App**

*Objective: Tag notes as “Work” or “Personal” using a simple ML API.*

### **Step 1 – Backend (FastAPI/Flask)**

* Prepare a small dataset (sample notes + tags).
* Train a simple ML model with **Scikit-learn Naive Bayes**.
* Save the model with `joblib`.
* Expose `/predict` endpoint → input: text, output: predicted tag.

### **Step 2 – Frontend (React Native)**

* Create a text input for entering notes.
* Add a “Classify” button.
* On press → send note to backend API.
* Display the returned tag (“Work” / “Personal”).

### **Step 3 – Final Touches**

* Show loading spinner while API call runs.
* Handle errors gracefully.
* Bonus: Store past classified notes in local storage (AsyncStorage).

👉 **Learning Outcome**:
By the end of Week 1, learners will know:

* Difference between AI, ML, DL, GenAI.
* How to set up and run a RN app.
* How to connect RN apps to APIs.
* How to integrate a simple AI backend into RN.

---

