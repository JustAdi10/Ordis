ai_assistant/  
│── speech_module/           # Handles all voice-related tasks  
│   ├── speech_to_text.py    # Whisper.cpp for speech recognition  
│   ├── text_to_speech.py    # Coqui TTS/VITS for voice responses  
│   ├── hotword_detection.py # Porcupine/Mycroft Precise for wake-word detection  
│── ai_core/                 # AI processing and memory  
│   ├── llm.py               # Local LLM (Mistral, Llama, Phi-2)  
│   ├── memory.py            # Context recall (FAISS + SQLite)  
│   ├── command_handler.py   # Parses input and executes relevant actions  
│── system_control/          # Interacts with the system  
│   ├── automation.py        # Runs CLI/system commands  
│   ├── app_control.py       # Opens/manages apps  
│   ├── file_manager.py      # Handles file operations  
│── cli_ui/                  # CLI interaction layer  
│   ├── cli.py               # Main CLI interface  
│   ├── background_tasks.py  # Async task handling (TTS, automation, etc.)  
│── config.py                # Global settings and paths  
│── requirements.txt         # Dependencies  
│── main.py                  # Entry point (initializes modules)  
│── README.md                # Documentation  