
# **LBSocial Chatbot**  

This project integrates an **AI-powered chatbot** into [LBSocial.net](https://lbsocial.net) using **Wix Chat and OpenAI Assistants API**. The chatbot retrieves answers from **LBSocial's YouTube video captions**, making it an **interactive learning assistant** for data analytics and AI topics.  

## **How the Chatbot Works**  

1. **Retrieve Video Captions from YouTube**  
   - A Python script (`video_captions_retrive.ipynb`) **fetches YouTube captions** using the YouTube API.  
   - The script was generated by **ChatGPT** and automates caption extraction.  
   - You can find LBSocial's YouTube videos here: [LBSocial YouTube Channel](https://www.youtube.com/channel/UCwtRYX-OsUj4VHLic2XQYog).  

2. **Upload Captions to OpenAI Vector Store**  
   - The extracted captions are **manually uploaded** to OpenAI as a **vector database** for retrieval.  

3. **OpenAI Assistant Processes Queries**  
   - An **OpenAI Assistant** is manually configured to **retrieve relevant captions** from the vector store.  
   - The AI’s **response instructions** were generated by **ChatGPT** to ensure accurate replies.  
   - Learn more about OpenAI Assistants here: [OpenAI Assistants Overview](https://platform.openai.com/docs/assistants/overview).  
   
   - **Thread-Based Conversations**: The assistant creates a unique **thread** for each user to maintain context during interactions, allowing for more personalized and relevant responses.  
   
4. **Wix Chatbot Implementation**  
   - A **Wix Chatbot** is deployed on **LBSocial.net**, enabling users to interact with the AI.  
   - **Frontend and backend files** for the chatbot were created using **ChatGPT**, referencing the YouTube tutorial:  

     📌 **[How to Turn the Native Wix Chat (App Market) into ChatGPT with OpenAI](https://www.youtube.com/watch?v=2Vn5fQjx4Y8&t=690s)**  
   
   - **User-Dedicated Channels**: On Wix, each user has a **dedicated channel**, ensuring chat history is organized and easily accessible for continued interactions.  
   
   - **Benefits of Thread-Based and Channel-Based Conversations**:  
     - **Personalized Experience**: Since the assistant tracks individual conversations, users receive more tailored responses.  
     - **Context Retention**: Instead of starting from scratch every time, the assistant remembers the context of past interactions.  
     - **Seamless Integration**: Users on Wix can continue discussions in their dedicated chat channels without losing important insights.  
   
---

## **Project Files & Their Functions**  

### **1. Backend & Frontend**  
- **`chatbot.jsw`** – Handles backend logic for the Wix chatbot, including OpenAI API communication.  
- **`front-end.js`** – Manages user interactions and displays responses in Wix Chat.  

### **2. OpenAI Assistant & Data Processing**  
- **`assistant-instructions.txt`** – Defines how the OpenAI Assistant retrieves YouTube captions and formats responses.  
- **`video_captions_retrive.ipynb`** – Python script (created by ChatGPT) that extracts captions from YouTube videos.  

### **3. Documentation & Licensing**  
- **`README.md`** – Project introduction and setup guide.  
- **`LICENSE`** – Open-source license for this repository.  

---

## **Key Features**  

✅ **AI-powered responses** – The chatbot provides answers based on **LBSocial's YouTube captions**.  
✅ **Relevant video links** – The chatbot shares **YouTube URLs** for deeper learning.  
✅ **Wix Chatbot Integration** – Users can interact with the assistant directly on **LBSocial.net**.  
✅ **Secure API Management** – Sensitive keys are **excluded from GitHub** for security.  
✅ **Thread & Channel-Based Conversations** – Personalized chat history ensures seamless interactions.  

---

## **License**  

This project is licensed under the **MIT License**. See `LICENSE` for details.  


