##  Key Features
  Enhanced Visual Design
- **Creative ASCII Art Header** - Professional, visually appealing welcome banner
- **Color-Coded Console Output** - Green (success), Cyan (info), Yellow (warnings), Red (errors)
- **Decorative Borders & Boxes** - Professional formatting throughout
- **Animated ASCII Display** - Engaging visual introduction

Voice Integration
- **Text-to-Speech Audio** - Professional voice greeting using Windows TTS
- **High-Quality Audio Generation** - greeting.wav file for immersive experience
- **Graceful Degradation** - App continues if audio unavailable
- **Professional Narration** - Clear, engaging audio greeting

 Personalized User Interaction
- **Name-Based Personalization** - All responses include user's name
- **Professional Greeting** - Warm, welcoming introduction
- **Session Tracking** - Message count and duration monitoring
- **Engaging Conversation Style** - Natural, helpful dialogue

Comprehensive Cybersecurity Responses
- **15+ Detailed Topics** covering:
  -  Password Safety & Creation
  -  Phishing Prevention & Detection
  -  Safe Browsing Practices
  -  Malware Protection & Defense
  - Two-Factor Authentication (2FA)
  -  Social Engineering Awareness
  -  Account Security Strategies
  - Email Security Best Practices
  -  Data Protection & Backup

  In-Depth Content
   - Each topic includes:
  - Multiple actionable tips
  - Real-world examples
  - Best practices
  - Common mistakes to avoid
  - Professional formatting with emojis
    
 Advanced Input Validation(Class4)
- **Comprehensive Validation** - Name validation with character checking
- **Graceful Error Handling** - Helpful, user-friendly error messages
- **Exception Management** - Try-catch blocks throughout
- **Security-Focused** - Prevents invalid input from affecting application

Interactive Command System
- **Topical Queries** - Ask about any cybersecurity topic
- **Special Commands** - help, clear, stats, exit, quit
- **Intelligent Matching** - Substring matching for topic recognition
- **Default Responses** - Helpful guidance for unknown queries

Session Management
- **Message Counter** - Tracks conversation activity
- **Session Duration** - Records time spent in session
- **Statistics Command** - View session summary anytime
- **Exit Summary** - Comprehensive farewell with session data


poe_p2
# Cybersecurity AI Assistant Terminal (POE Part 2)

An interactive, matrix-themed WPF educational application written in C# designed to mentor users on core cybersecurity vulnerabilities, analyze conversational sentiments, and test operational retention using dynamic assessment frameworks.

---

##  Architecture & Separation of Concerns
The application strictly follows the **Single Responsibility Principle (SRP)** by separating logic engines entirely away from the user interface boundaries:

1. **`MainWindow.xaml.cs`** - Orchestrates UI view grids, element visibilities, and terminal logs.
2. **`AudioManager.cs`** - Generates and streams background speech synthesis wave files natively.
3. **`SentimentAnalyzer.cs`** - Evaluates input strings for user mood states (worried, frustrated, curious).
4. **`TopicDetector.cs`** - Houses the dictionary libraries explaining phishing, malware, and injection types.
5. **`MemoryManager.cs`** - Directly handles flat file-system persistence (`memory.txt`) for tracking user interests.
6. **`QuizManager.cs`** - Builds evaluation objects, evaluates user answers, and tracks grading metrics.

---

##  Features Breakdown
* **Dynamic Content Mapping:** Identifies hidden cybersecurity technical keywords in human conversations.
* **Empathetic AI Core:** Adapts the bot output header depending on the user's frustration or worry patterns.
* **Audio Welcome Integration:** Auto-synthesizes a hardware-independent native `.wav` audio greeting upon login confirmation.
* **Interactive Assessment Module:** Generates focused interactive multiple-choice tests targeting the user's latest historical interactions.
* **State Persistence:** Stores tracking parameters locally to remember favorite topics between individual sessions.

---

##  Installation & Setup Instructions

### Prerequisites
* Windows 10/11 OS
* Visual Studio (2022 recommended)
* **.NET Framework 4.7.2+** or **.NET Core 6.0/8.0** workload configuration

### Running the Project
1. Open the project solution (`poe_p2.sln`) inside Visual Studio.
2. Ensure `System.Speech` is referenced properly inside your project reference explorer nodes.
3. Verify that the file paths pointing to the media resources inside `AudioManager.cs` coordinate cleanly with your local user configuration directories.
4. Press `F5` or click **Start / Debug** to spin up the application terminal shell workspace.

---

## Unit Testing Core Logic
The stability of our decoupled classes is validated using an **MSTest Core Framework** suite project (`poe_p2_tests`). 

### Running Automated Diagnostic Tests:
1. Navigate to the top taskbar options inside Visual Studio and select **Test** -> **Run All Tests**.
2. Open your project **Test Explorer** tab (`Ctrl + E, T`) to view execution status profiles covering sentiment detections, database lookups, and score processing counters.
