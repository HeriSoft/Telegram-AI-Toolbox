Instructions for finding and configuring API Keys for File .ENV

Welcome to BOT! For BOT to operate, you need to provide personal keys APIs and configuration information in the file '.env`. Here are detailed instructions to get each key and how to fill them into the file '.env`.
App Version: 1.0.8
---
First:
/// Download Get cookies.txt LOCALLY extension
https://chromewebstore.google.com/detail/get-cookiestxt-locally/cclelndahbckbenkjhflpdbgdldlbecc

### 1. Openai_api_key
- ** Description **: API lock to use Openai services (such as chatgpt).
- ** How to get **:
  1. Visit https://platform.openai.com/.
  2. Register/log in account.
  3. In the "API Keys" section in Dashboard.
  4. Click "Create New Secret Key", copying the key created.
- ** fill in .env **:
  Openai_api_key = Your_openai_key_here

---

### 2. Google_api_key
- ** Description **: API lock to use Google services (such as Google Custom Search).
- ** How to get **:
  1. Visit https://console.cloud.google.com/.
  2. Create a new project (or select the existing project).
  3. Go to "APIS & Services"> "Creditials".
  4. Click "Create Credit"> "API Key", copy the key.
- ** fill in .env **:
  Google_api_Key = Your_google_api_key_here

---

### 3. Search_engine_id
- ** Description **: ID of custom search engine (used with Google Custom Search).
- ** How to get **:
  1. Visit https://cse.google.com/cse/all.
  2. Login and create a "Custom Search Engine".
  3. After creating, go to "Edit Search Engine"> "Basics", copy "Search Engine ID".
- ** fill in .env **:
  Search_engine_id = Your_search_engine_id_here

---

### 4. Gemini_api_key
- ** Description **: API Lock for Google Gemini (if bot uses this model).
- ** How to get **:
  1. Visit: "https://aistudio.google.com/apikey" to get API. Check https://cloud.google.com/ or Google ai Documents to update.
  2. If Available, Create the same key as google_api_key in Google Cloud Console.
- ** fill in .env **:
  Gemini_api_key = Your_gemini_api_key_here

---

### 5. Google_cloud_Project_id
- ** Description **: ID of Google Cloud project to use services like Vertex AI.
- ** How to get **:
  1. Visit https://console.cloud.google.com/.
  2. Create or choose a project.
  3. The project ID is at the top of Dashboard (for example, "My-Project-123").
- ** fill in .env **:
  Google_Cloud_Project_ID = Your_Project_id_Here

---

### 6. Google_Cloud_location
- ** Description **: The geographical area of ​​Google Cloud service (default is "US-CENTRAL1").
- ** How to get **:
  - No need to create, use the default "US-CENTRAL1" value unless you need another area (see Google Cloud document).
- ** fill in .env **:
  Google_Cloud_location = US-CENTRAL1

---

### 7. Google_application_Creditials
- ** Description **: The path to the JSON file contains Google Cloud service account information.
- ** How to get **:
  1. Visit https://console.cloud.google.com/.
  2. Go to "APIS & Services"> "Creditials".
  3. Click "Create Credentials"> "Service Account", fill out information and create.
  4. Download JSON file (for example: "Service-account-key.json") and save it to the device (for example: D: \ path-to-your-folder \).
- Important note: It is necessary to activate Vertex's Imagen 3 service for the service account to use the high quality image creation function by Model Imagen 3
- ** fill in .env **:
  Google_application_Credentials = D: \\ path-to-Your-Folder \\ Service-account-KEY.JSON
  (Change the path according to your JSON file position)

---

### 8. Telegram_bot_token
- ** Description **: token to connect BOT to Telegram.
- ** How to get **:
  1. Open the Telegram application, find "@botfather".
  2. Send orders /newbot, follow the instructions to create BOT.
  3. After creating, Botfather will provide token ("123456: ABC-DEF1234GHIKL-Jzyx57W2V1U123ew11").
- ** fill in .env **:
  Telegram_bot_token = Your_telegram_bot_token_here

---

### 9. Elevenlabs_api_key
- ** Description **: API lock to use the text transfer service into Elevenlabs voice.
- ** How to get **:
  1. Visit https://elevenlabs.io/.
  2. Register/log in account.
  3. Go to "Profile" or "API Keys", create and copy key.
- ** fill in .env **:
  Elevenlabs_api_key = Your_elevenlabs_api_key_here

---

### 10. Elevenlabs_voice_1, elevenlabs_voice_2, elevenlabs_voice_3
- ** Description **: ID of specific voices from Elevenlabs.
- ** How to get **:
  1. Login to Elevenlabs.
  2. Go to "Voices" or "voice lab", choose the voice you want.
  3. Copy the voice of the voice (usually a series of characters as "21m00tcm4tlvdq8ikwam").
- ** fill in .env **:
  Elevenlabs_voice_1 = Your_voice_id_1_here
  Elevenlabs_voice_2 = Your_voice_id_2_here
  Elevenlabs_voice_3 = Your_voice_id_3_here

---

### How to use .NV file
1. Create a text file `` .env` in the same folder with `bot.exe`.
2. Copy the lines below to the file '.env` and fill your information:

Openai_api_key = Your_openai_key_here
Google_api_Key = Your_google_api_key_here
Search_engine_id = Your_search_engine_id_here
Gemini_api_key = Your_gemini_api_key_here
Google_Cloud_Project_ID = Your_Project_id_Here
Google_Cloud_location = US-CENTRAL1
Google_Application_Credentials = D: \ Path-to-Your-Folder \ Service-Account-Key.json
Telegram_bot_token = Your_telegram_bot_token_here
Elevenlabs_api_key = Your_elevenlabs_api_key_here
Elevenlabs_voice_1 = Your_voice_id_1_here
Elevenlabs_voice_2 = Your_voice_id_2_here
Elevenlabs_voice_3 = Your_voice_id_3_here
KEY_UNLOCKER= Key-for-user
KEY_UNLOCKER_ADMIN= Key-for-admin

3. Save the file and run `bot.exe`.

---

### Note
- Keep secret keys APIs, do not share file `.env` public.
- If you encounter errors when running BOT, check the key and path in `.env`.

Wish you success!