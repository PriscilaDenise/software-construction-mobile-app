
# *APPLICATION*: WHATSAPP

# Part A (Understanding the App)

What problem does the app solve?

●	High-cost international texting

●	Restrictive SMS charges

● Complicated user identification 

●	Ad-free Experience 

Who are the primary users?

- Smartphone users
  
- Students
  
- Enterprise users
# Core features.
- Instant messaging
- Voice and video calling
- Group Chats
- Media sharing
- Voice notes
- Message forwarding
- Status updates


# Part B: Thinking Behind the Scenes

This document explains how core WhatsApp features work behind the scenes. It outlines the key software components involved, internet connectivity requirements, and the system behavior when the network is slow or unavailable.



## Instant Messaging

**Software Components Involved**
- **User Interface (UI):** Chart screen, Text input box, send button

  
**Business Logic:**
  - Message sending and receiving
  - Time-stamping of messages
  - message delivery status indicators (✓, ✓✓)
    
- **Network / APIs:** Transmits messages via WhatsApp servers to recipients

 **Data Storage:**
  - Local storage on the device
  - Server-side storage until delivery

**Internet Connectivity Required**: Yes


**Behavior When Network Is Slow or Unavailable:**
- Messages remain in a sending state with no tick (delivery status indicator )
- Message delivery is delayed



##  Voice and Video Calling

**Software Components Involved**
**User Interface (UI):** Call screen, Mute button, Speaker controls, Video display
 
**Business Logic:**  Manages audio and video switching when on a call
    
**Network / APIs:** Supports real-time communication using internet protocols

**Internet Connectivity Required**: Yes


**Behavior When Network Is Slow or Unavailable:**
- Reduced audio and video quality
- Calls may drop or fail to connect
- Freezing and latency during calls



##  Group Chats

**Software Components Involved**

**User Interface (UI):** Group chat interface, Participant list, Admin controls
  
**Business Logic:**
  - Manages group membership and permissions
  - Handles message distribution while managing permissions, delivery status, and message order
    
**Network / APIs:** Sends messages to multiple recipients simultaneously
    
**Data Storage:** Stores group messages and metadata

**Internet Connectivity Required:** Yes

**Behavior When Network Is Slow or Unavailable:** Messages are delivered late



##  Media Sharing (Photos, Videos, Documents)

**Software Components Involved**

**User Interface (UI):** Media picker, Preview screen, Download button
  
**Business Logic:**
  - Compresses media files
  - Validates file size and format
    
**Network / APIs:** Handles media uploads and downloads
  
**Data Storage:** Stores media locally and temporarily on servers

**Internet Connectivity Required:** Yes

**Behavior When Network Is Slow or Unavailable:**
- Uploads and downloads may pause or fail
- Media transmission takes longer
- Media may remain stuck loading



##  Voice Notes

**Software Components Involved**

**User Interface (UI):** Microphone button, playback controls
  
**Business Logic:**
  - Records and compresses audio
  - Manages playback
    
**Network / APIs:** Transmits audio files over the internet
  
**Data Storage:** Saves voice notes on both device and server

**Internet Connectivity Required:** Yes (for sending and receiving)

**Behavior When Network Is Slow or Unavailable:**
- Voice notes send slowly
- Playback may buffer
- Sending resumes once internet connectivity is restored



##  Message Forwarding

**Software Components Involved**
- **User Interface (UI):** Foward button, Contact selection screen
  
- **Business Logic:**
  - Copies message content
  - Restricts bulk forwarding
    
- **Network / APIs:** Resends messages to selected recipients
  
- **Data Storage:** Uses existing stored message data

**Internet Connectivity Required:** Yes

**Behavior When Network Is Slow or Unavailable:**
- Forwarding delays occur
- Messages remain unsent
- Forwarding completes after network recovery



##  Status Updates

**Software Components Involved**
- **User Interface (UI):** Status Viewer, Camera interface, Text editor
  
- **Business Logic:**
  - Enforces 24-hour status showing expiration
  - Manages privacy settings
    
- **Network / APIs:** Uploads and retrieves status content
  
- **Data Storage:** Temporarily stores status data until expiration

**Internet Connectivity Required:**  Yes

**Behavior When Network Is Slow or Unavailable:**
- Status uploads are delayed or fail
- Status viewing is unavailable
- Status uploads automatically once the user reconnects

# Part C: Change and Maintainability
- **Optimize the app for low-end smartphones**
- Reason: A suitable change scenario for WhatsApp is optimizing the app for low-end smartphones. This change would improve performance, reduce resource usage, and increase accessibility for users in developing countries such as Uganda.

# Which parts of the app would need changes?
First, the **user interface (UI)** would need changes. Low-end phones struggle with heavy animations, high-resolution images, and complex transitions. To improve performance, the app would need simpler layouts, fewer visual effects, and lighter icons so the phone’s processor and memory are not overloaded.

Second, the media handliing system would need adjustment. Sending and receiving photos, videos, and voice notes uses a lot of memory and storage on low-end devices. WhatsApp would need to compress media more aggressively and limit how much media is stored on the phone at once. 

Third, background processes such as message syncing, notifications, and backups would need optimisation.Low-end phones often kill apps running in the background to save memory. WhatsApp would have to reduce background activity so the app does not slow down the entire device or drain the battery.

Finally, storage and caching logic would need improvement. Many low-end phones have very little free storage, so WhatsApp would need to clean old data automatically and avoid keeping unnecessary files.

# What existing features could break?
When optimizing for low-end smartphones, some features may not work exactly as users expect.

Media-related features could be affected first. Stronger compression may make photos and videos appear lower in quality, which some users may notice and dislike.

Voice and video calls could also suffer. To save processing power and data, calls may run at lower audio or video quality, leading to less clear conversations.

Another issue could be delayed notifications. If background activity is reduced too much, messages may not appear instantly, especially when the phone is locked or low on memory.

Visual features like animations and smooth transitions might be removed or simplified. While this improves performance, the app may feel less modern to some users.

# Why would this change be difficult to implement?
This change is difficult mainly because of the huge variety of devices WhatsApp runs on. Low-end smartphones differ greatly in RAM size, processor speed, Android versions, and storage capacity.

If WhatsApp removes too many features or reduces quality too much, users may feel the app has become worse, even if it runs faster and fail to balance performance and user experience.

Developers may need to treat low-end and high-end devices differently, which increases complexity and makes bugs more likely.

This change would require extensive testing. Every optimization must be tested on real low-end devices to ensure the app does not crash, lose messages, or behave unpredictably.

# Part D: Software Construction Challenges

**1. Performance and Scalability**
As the user base grows, WhatsApp is required to process a massive number of messages, calls, and media transfers at the same time, which places heavy pressure on the system. Because all users expect instant communication, even a very small delay can quickly become noticeable and frustrating when it affects millions of people simultaneously. 

**2. Security and Data Privacy**
WhatsApp faces the significant challenge of protecting highly sensitive user data, as they store and transmit private conversations that make them prime targets for cyberattacks. Any security flaw, even minor, can expose personal information and severely damage user trust. The complexity of implementing robust end-to-end encryption while maintaining performance adds another layer of difficulty.


**3. Testing Across Devices and OS Versions**
WhatsApp faces the challenge of ensuring consistent functionality across a vast array of devices, operating systems, and software versions. A feature that works perfectly on one phone may fail on another due to differences in hardware, screen sizes, or OS behavior. Additionally, operating system updates can unexpectedly break existing features, creating further unpredictability. Testing every possible combination of devices, OS versions, and app states is extremely time-consuming and resource-intensive, making it a continuous and complex challenge to ensure the app works reliably for all users.

**4. Backward Compatibility**
WhatsApp faces the challenge of maintaining backward compatibility because not all users update their apps or devices regularly. New features must function correctly on older versions of the app, and some older devices may lack the hardware or software capabilities to support these updates. This creates a complex situation where failing to support legacy devices risks excluding a significant portion of users, while ensuring compatibility adds an extra burden to development and testing efforts.

**5. Reliability Under Poor Network Conditions**
WhatsApp faces the challenge of ensuring reliable operation in areas with unstable internet connections. In such conditions, messages can fail to send or arrive out of order, while calls may drop or experience significant delays. These network issues make it difficult to provide a consistent and seamless user experience, as the app must remain functional despite interruptions and fluctuations in connectivity. 



