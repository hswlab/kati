# KATI-AI Chat (Bing Chat)
[![GitHub](https://img.shields.io/github/license/hswlab/kati)](https://github.com/hswlab/kati/blob/main/LICENSE) 
[![Downloads](https://img.shields.io/github/downloads/hswlab/kati/total)](https://github.com/hswlab/kati/releases/latest) 
[![Downloads](https://img.shields.io/github/v/release/hswlab/kati)](https://github.com/hswlab/kati/releases/latest) 

KATI is a simple desktop application that allows you to quickly and easily have a conversation with an 
AI. The C# library BingChatApi is used to communicate with the AI. The app is continuously being 
developed. In the first version, a simple text-based conversation is already possible. The application 
can be installed on Windows, but is expected to be available for Linux as well.

![preview](https://github.com/hswlab/kati/blob/main/Screenshot.png)

# Nuget packages and associated licenses used in kati
- Newtonsoft.Json <a href="https://licenses.nuget.org/MIT">`license`</a>
- Esprima <a href="https://licenses.nuget.org/BSD-3-Clause">`license`</a>
- ElectronNET.API <a href="https://licenses.nuget.org/MIT">`license`</a>
- LiteDB <a href="https://www.nuget.org/packages/LiteDB/5.0.16/license">`license`</a>
- BingChatApi <a href="https://github.com/liaosunny123/BingChatApi/blob/master/license">`license`</a>

# More Details
- German: https://github.com/hswlab/kati/blob/main/about-de.pdf
- English: https://github.com/hswlab/kati/blob/main/about-en.pdf

# Known issues
- The AI doesn't send a response: I've noticed that this sometimes happens when the VPN is 
enabled. Disable VPN if it is enabled and restart the application.
- The AI sends an incomplete response: In the case of links, code, special characters, or if the 
AI's response is too long, the response sometimes does not arrive in full. Explain to the AI 
that its last response is incomplete, it will then try to send its response in a different way.
