
# *APPLICATION*: WHATSAPP

# Part A (Understanding the App)

What problem does the app solve?

●	High-cost international texting

●	Restrictive SMS charges

Who are the primary users?

- Smartphone users
  
- Students
  
- Enterprise users
# Core features.


# Part B: Thinking Behind the Scenes

This document explains how core WhatsApp features work behind the scenes. It outlines the key software components involved, internet connectivity requirements, and the system behavior when the network is slow or unavailable.



## Instant Messaging

**Software Components Involved**
- **User Interface (UI):**
  - Chat screen
  - Text input box
  - Send button
- **Business Logic:**
  - Message sending and receiving
  - Time-stamping of messages
  - message delivery status indicators (✓, ✓✓)
- **Network / APIs:**
  - Transmits messages via WhatsApp servers to recipients
- **Data Storage:**
  - Local storage on the device
  - Server-side storage until delivery

**Internet Connectivity Required**
- Yes

**Behavior When Network Is Slow or Unavailable**
- Messages remain in a sending state with no tick (delivery status indicator )
- Message delivery is delayed



##  Voice and Video Calling

**Software Components Involved**
- **User Interface (UI):**
  - Call screen
  - Mute button
  - Speaker controls
  - Video display
- **Business Logic:**
  - Manages audio and video switching when on a call
- **Network / APIs:**
  - Supports real-time communication using internet protocols

**Internet Connectivity Required**
- Yes

**Behavior When Network Is Slow or Unavailable**
- Reduced audio and video quality
- Calls may drop or fail to connect
- Freezing and latency during calls



##  Group Chats

**Software Components Involved**
- **User Interface (UI):**
  - Group chat interface
  - Participant list
  - Admin controls
- **Business Logic:**
  - Manages group membership and permissions
  - Handles message distribution while managing permissions, delivery status, and message order
- **Network / APIs:**
  - Sends messages to multiple recipients simultaneously
- **Data Storage:**
  - Stores group messages and metadata

**Internet Connectivity Required**
- Yes

**Behavior When Network Is Slow or Unavailable**
- Messages are delivered late



##  Media Sharing (Photos, Videos, Documents)

**Software Components Involved**
- **User Interface (UI):**
  - Media picker
  - Preview screen
  - Download button
- **Business Logic:**
  - Compresses media files
  - Validates file size and format
- **Network / APIs:**
  - Handles media uploads and downloads
- **Data Storage:**
  - Stores media locally and temporarily on servers

**Internet Connectivity Required**
- Yes

**Behavior When Network Is Slow or Unavailable**
- Uploads and downloads may pause or fail
- Media transmission takes longer
- Media may remain stuck loading



##  Voice Notes

**Software Components Involved**
- **User Interface (UI):**
  - Microphone button
  - Playback controls
- **Business Logic:**
  - Records and compresses audio
  - Manages playback
- **Network / APIs:**
  - Transmits audio files over the internet
- **Data Storage:**
  - Saves voice notes on both device and server

**Internet Connectivity Required**
- Yes (for sending and receiving)

**Behavior When Network Is Slow or Unavailable**
- Voice notes send slowly
- Playback may buffer
- Sending resumes once internet connectivity is restored



##  Message Forwarding

**Software Components Involved**
- **User Interface (UI):**
  - Forward button
  - Contact selection screen
- **Business Logic:**
  - Copies message content
  - Restricts bulk forwarding
- **Network / APIs:**
  - Resends messages to selected recipients
- **Data Storage:**
  - Uses existing stored message data

**Internet Connectivity Required**
- Yes

**Behavior When Network Is Slow or Unavailable**
- Forwarding delays occur
- Messages remain unsent
- Forwarding completes after network recovery



##  Status Updates

**Software Components Involved**
- **User Interface (UI):**
  - Status viewer
  - Camera interface
  - Text editor
- **Business Logic:**
  - Enforces 24-hour expiration
  - Manages privacy settings
- **Network / APIs:**
  - Uploads and retrieves status content
- **Data Storage:**
  - Temporarily stores status data until expiration

**Internet Connectivity Required**
- Yes

**Behavior When Network Is Slow or Unavailable**
- Status uploads are delayed or fail
- Status viewing is unavailable
- Status uploads automatically once the user reconnects





