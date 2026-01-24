
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







