# Vizor.Sendkbd

[![Release](https://img.shields.io/github/v/release/VizorAX/sendkbd)](https://github.com/VizorAX/sendkbd/releases)
[![License](https://img.shields.io/github/license/VizorAX/sendkbd)](LICENSE)

> **Vizor.Sendkbd** includes both `vizor.sendkbd.exe` and `vizor.recvkbd.exe` for efficient, low-latency keyboard event streaming over a network.

🌟 **Key Features**
-------------------

*   🖥️ **Low-Latency Keyboard Event Streaming**: Stream keyboard input and keypress events in real time over the network.
*   🎯 **Comprehensive Remote Control**: Supports all keyboard events to provide seamless interaction with a remote machine.
*   ⚡ **Performance-Optimized**: Built to handle keyboard events with minimal delay for smooth and responsive typing experiences.

📥 **Download and Installation**
-------------------------------

### **Requirements**

*   **Operating System**: Windows 10 or later (Untested on other Windows versions)
*   **Disk Space**: At least 50 MB of free space

### **Dependencies**

*   **None**: Utilizes pure WinAPI functionality.

### **Installation Steps**

1.  **Download the Latest Release**: Grab the executables from the [Releases](https://github.com/VizorAX/sendkbd/releases) page.
    
2.  **Extract the Package**:
    *   Unzip the downloaded package to your desired directory.
    
3.  **Run the Executables**:
    *   **To Stream Keyboard Events**: `vizor.sendkbd.exe <streamer_port> <receiver_address> <receiver_port>`
    *   **To Receive Keyboard Events**: `vizor.recvkbd.exe <receiver_port> <streamer_address> <streamer_port>`

4.  **Launch the Application**:
    *   After running the commands, the executables will handle the streaming and reception of keyboard inputs and events as per the provided parameters.

📖 **Usage Examples**
---------------------
### Streaming Keyboard Data and Events
```bash
vizor.sendkbd.exe 7000 192.168.1.100 8000
```
- Streaming keyboard inputs from port `7000` to a receiver at address `192.168.1.100` on port `8000`.

### Receiving Keyboard Data and Events
```bash
vizor.recvkbd.exe 8000 192.168.1.50 7000
```
- Receiving keyboard inputs on port `8000` from a streamer at address `192.168.1.50` on port `7000`.

🛠️ **Troubleshooting**
-----------------------
If you run into any issues, here are some steps to try:

*   **Check for Updates**: Make sure you're using the latest version from the [Releases](https://github.com/VizorAX/sendkbd/releases) page.
*   **Verify Network Configuration**: Ensure the network settings are configured correctly on both ends of the stream.
*   **Verify Parameters**: Double-check the command-line arguments to make sure everything is correct.
*   **Contact Support**: Reach out to [sansorich@gmail.com](mailto:sansorich@gmail.com) with any issue details.

📄 **License**
--------------
This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for more details.

📧 **Contact**
--------------
- **Rodrigo R. S. Sorgato**: [LinkedIn](https://www.linkedin.com/in/rrssorgato) | [Email](mailto:sansorich@gmail.com)
