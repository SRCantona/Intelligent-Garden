<!--
  README.md for the "Intelligent Garden" Concept
  ------------------------------------------------
  This is a template/placeholder for a GitHub repo.
  No implementation exists—this is purely a design idea.
-->

# 🌱 Intelligent Garden

## 📖 Introduction
Welcome to **Intelligent Garden**, an innovative concept designed to transform the way gardeners—both hobbyists and professionals—interact with their plants. By leveraging AI-powered image analysis and a vibrant community platform, our app will:

- Diagnose plant health issues in real time
- Offer personalized care recommendations
- Foster community-driven knowledge sharing and collaboration

---

## 🎯 Vision & Scope

- **Goal**: Empower both hobbyist and professional gardeners with instant plant diagnostics, crowd‑sourced wisdom, and social collaboration.  
- **Status**: 💡 _Idea only_ — no code or prototype yet.  
- **Target Platforms**: Android  & iOS 

---

## 🌟 Advantages

1. **Instant Insight**: Quickly identify plant species and health concerns without specialist equipment.
2. **Personalized Care**: Receive tailored watering, fertilization, and pruning schedules based on real data.
3. **Knowledge Sharing**: Tap into a community of gardeners to crowdsource solutions and best practices.
4. **Historical Tracking**: Maintain a digital log of past scans and growth metrics to analyze trends over time.
5. **Scalable Architecture**: Designed for modular expansion—add new sensors, AI models, or community features as needed.

---

## 🚀 Features

- **🔍 Plant Scan**  
  - Take or upload photos of plants/soil  
  - AI‑powered analysis for species ID, health status & care tips  
- **💬 Community Hub**  
  - Real‑time chat, posts, comments & upvotes  
  - “Trusted” badges for expert gardeners  
- **👤 Profiles & Badges**  
  - User sign‑up/sign‑in via email/password  
  - Admin vs. normal user roles & privileges  
- **📊 Historical Data**  
  - Save scan history, notes, and growth metrics  

---

## 💬 Community Concept

The heart of Intelligent Garden is its gardener community:

- **Collaborative Q&A**: Post questions with images; receive answers from enthusiasts and experts.
- **Reputation System & Badges**: 
  - `Novice`: New users just getting started.
  - `Green Thumb`: Experienced hobbyists with solid contributions.
  - `Trusted (Expert)`: Recognized plant experts and verified horticulturists.
- **Localized Forums**: Join regional groups to discuss climate-specific challenges and plant species.
- **Events & Challenges**: Participate in seasonal photo contests, grow-offs, and seed exchanges.

This social layer not only aids problem-solving but also encourages ongoing engagement and learning.

---
### 📐 System Architecture

- **Layered Approach**:  
  - **UI Layer** – Mobile app screens & navigation  
  - **Monitoring Layer** – Sensor integrations (camera), image processing  
  - **Decision Layer** – AI inference (YOLO model + GPT‑style reports)  
  - **Control Layer** – Actuator hooks (e.g., watering alerts)  
  - **Security Layer** – Auth & secure comms  
  - **Data Layer** – Historical data & logs  



---

## 🎨 User Interface Design

UI/UX philosophy focuses on simplicity, clarity, and engagement. 

- **Login Page Interface**
  ![image](https://github.com/user-attachments/assets/2e7a8843-9f6b-42ca-98f0-b6565cd04c33)

- **Create Account Interface**
  ![image](https://github.com/user-attachments/assets/e656ee41-faa2-4a37-9bd4-7ac1903013c0)

- **Forgot Password Interface**
  ![image](https://github.com/user-attachments/assets/5576fff1-2696-4f84-a5fc-599a85b8a652)
  ![image](https://github.com/user-attachments/assets/dfc6adba-8c55-4a44-b1d2-94190c5f9180)

- **Home Interface**
  ![image](https://github.com/user-attachments/assets/cd1b36f7-8e79-4941-8ff7-1b1b992c68c7)

- **Explore Interface**
  ![image](https://github.com/user-attachments/assets/7c79801c-16ed-4929-a92a-8299890fc71c)

- **Camera Interface**
  ![image](https://github.com/user-attachments/assets/f3069d84-444f-487f-861b-02158c62ca2a)
  ![image](https://github.com/user-attachments/assets/2e3c0dae-2851-4ad6-a1c0-cae595122ddf)

- **Community Interface**
  ![image](https://github.com/user-attachments/assets/33a1063e-8d80-4729-831c-6b174b2e8856)

- **Profile Interface**
  ![image](https://github.com/user-attachments/assets/f2651b02-f81a-4ddd-baba-023282310966)
  ![image](https://github.com/user-attachments/assets/28c61f49-6d27-48f1-9893-e74525173719)


---
### 🔍 Scan Workflow

The **Plant Scanner** module works as follows:

| Prerequisite | Have an account and valid login credentials |
|--------------|----------------------------------------------|
| **Test Procedure** | 1. Open the **Camera Interface** and tap “Scan”.<br>a) If the image is clear, proceed to inference.<br>b) If the image is blurry, display an error: “Please take another picture and make sure it is not blurry.”<br>c) If the plant is not recognized, display: “Plant not recognized. Please upload the image to the community so that people can help identify it.” |
| **Expected Result** | a) Clear image: Display plant info and care recommendations.<br>b) Blurry image: Show blur warning message.<br>c) Unknown plant: Prompt user to share with the community. |

---
### 🗄️ Data Model

- **Entities**: User, Plant, Scan, Post, Comment, Moderator, BanRecord
![image](https://github.com/user-attachments/assets/531a51ba-8e83-4963-a9c6-7b428fd5a9e1)

- **ER Diagram** & **Relational Schema**

![image](https://github.com/user-attachments/assets/bbd678ef-23f9-46b9-9717-221c259a8b8b)



