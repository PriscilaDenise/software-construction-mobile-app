
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









