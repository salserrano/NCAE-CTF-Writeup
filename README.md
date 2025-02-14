<p align="center">
<img src="https://dots.neit.edu/cybercenter/wp-content/uploads/sites/42/2021/11/Capto_Capture-2021-11-19_01-41-20_PM.png"/>
</p>

# CTF Challenge Write-Up: Reverse Engineering and Hidden Secrets

Welcome to my CTF challenge write-up! While this competition took place two years ago, the skills I gained and the lessons I learned remain highly relevant to my work and passion for cybersecurity today. Below, I’ll walk you through two exciting challenges I solved during the competition, showcasing my problem-solving abilities, technical expertise, and determination. Let’s dive in!

---

## **Reverse Engineer CTF Challenge**

### **Challenge Overview**
We were provided with a text file containing cryptic code. After analyzing it, I identified it as **MIPS assembly code**. My goal was to reverse engineer the code and uncover the hidden flag.

**Code Text File**: [View the MIPS Code](https://textdoc.co/3CNVQpb4xeUk1o0D)

### **Tools Used**
- **QtSpim**: A MIPS simulator to execute the assembly code.
- **ChatGPT**: Assisted in identifying the code as MIPS assembly.

### **Approach**
1. **Identifying the Code**: With the help of ChatGPT, I recognized the text file as MIPS assembly code.
2. **Setting Up QtSpim**: I researched and installed QtSpim to run the code.
3. **Running the Code**: Upon execution, the program prompted for a password, which I didn’t have.

   ![Console after running the code](https://i.imgur.com/DN98nNw.png)  
   *The console output after running the code, showing the password prompt.*

4. **Single-Step Execution**: I used QtSpim’s **"Single Step"** feature to manually execute the code line by line, observing the output at each step.

   ![Single Step Option in QtSpim](https://i.imgur.com/K2hMGDK.png)  
   *The "Single Step" option in QtSpim, which allowed me to execute the code manually.*

5. **Discovering the Flag**: After meticulously stepping through the code, I reached the final line, which revealed the **flag** without requiring the password.

   ![Flag Found in QtSpim](https://i.imgur.com/h6S405c.jpeg)  
   *The flag revealed in QtSpim, circled in red for clarity.*

### **Key Takeaways**
- Gained hands-on experience with MIPS assembly and reverse engineering.
- Learned to use QtSpim for low-level code execution.
- Demonstrated persistence and problem-solving skills.

---

## **Kitty JPG File CTF Challenge**

### **Challenge Overview**
I was given a JPEG file that seemed suspicious. My task was to uncover any hidden data or flags within the file.

### **Tools Used**
- **WinRAR**: A file archiver utility to inspect the JPEG file.
- **Google**: Researched common passwords and file analysis techniques.

### **Approach**
1. **Initial Analysis**: Noticed the JPEG file behaved unusually, prompting further investigation.
2. **Inspecting with WinRAR**: Opened the file in WinRAR and discovered it was an **archived file** containing two text files:
   - `Flag.txt`: Password-protected.
   - `Memo.txt`: Contained the hint, *"Use the Least Common Passwords."*
3. **Cracking the Password**: Researched commonly used passwords and tried `123456`, which successfully unlocked `Flag.txt`.
4. **Retrieving the Flag**: Accessed the flag hidden within the file.

### **Key Takeaways**
- Learned how files can hide data using archiving techniques.
- Practiced password cracking using real-world knowledge of common passwords.
- Improved my ability to follow clues and think critically.

---

## **Reflection and Relevance Today**

While this competition happened two years ago, the skills I developed during these challenges have had a lasting impact on my technical abilities and mindset. Here’s why this experience remains relevant:

- **Foundational Skills**: Working with MIPS assembly and reverse engineering laid the groundwork for my understanding of low-level programming and system internals.
- **Problem-Solving Mindset**: The persistence and creativity I demonstrated during these challenges continue to guide my approach to solving complex problems.
- **Cybersecurity Awareness**: The Kitty JPG challenge taught me how files can hide data, a concept I’ve since applied in real-world security scenarios.

Since then, I’ve continued to build on these skills through personal projects, additional CTF competitions, and professional development. This write-up serves as a testament to my growth and passion for cybersecurity.

---

## **Conclusion**

These CTF challenges were a fantastic opportunity to apply my technical knowledge and problem-solving skills in a real-world context. Even though they took place two years ago, the lessons I learned and the skills I developed continue to shape my approach to cybersecurity and reverse engineering. I’m excited to share this write-up as a reflection of my journey and growth in the field.
