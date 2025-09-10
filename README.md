#  AI Media File Manager Agent

A simple AI-powered agent built in **Jupyter Notebook** that can manage your local files.  
It uses **Google Gemini** for natural language understanding and can:

-  List files in the current directory or sub-directories  
-  Read text files (`.txt`, `.py`, `.md`, `.json`, etc.)  
-  Play audio files (e.g., `.mp3`)  
-  Play video files (e.g., `.mp4`)  
-  Open documents with the default system application  

---

##  Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/media-file-agent.git
   cd media-file-agent
2. Create and activate a virtual environment
    ```
    python3 -m venv venv
    source venv/bin/activate   # On macOS/Linux
    venv\Scripts\activate      # On Windows


4. Install dependencies
    ```
    pip install google-generativeai jupyter python-dotenv


5. Set up your Gemini API key
    ```
    echo "GOOGLE_API_KEY=your_api_key_here" > .env


6. Launch Jupyter Notebook
    ```
    jupyter notebook


7. Open the notebook file (e.g., media_agent.ipynb).
    
      Run the cells to start the agent.

 #Usage

  When the agent starts, you can type natural language commands such as:

    "list files in current directory"
    
    "show me what's in Downloads"
    
    "read notes.txt"
    
    "play music.mp3"
    
    "open document.pdf"
  
    "change to home directory"

    Type quit to exit.

 #Requirements

    Python 3.8+
    
    Google Gemini API Key (from Google AI Studio
    )
    
    A media player installed (e.g., VLC, mpv, or system default opener)

# Notes

Text file reading is limited to the first 1000 characters (to keep outputs manageable).

The agent relies on your system’s default apps for opening/playing files.

Works best on Linux/macOS (Windows may require adjusting subprocess calls).

# Future Improvements

Add persistent memory of previous sessions

Support file search by keywords

Extend support for more file formats

**smith-odero**
