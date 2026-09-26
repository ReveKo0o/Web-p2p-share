# Web-P2P-Share

<img width="878" height="454" alt="image" src="https://github.com/user-attachments/assets/c3594191-dc16-4371-8886-2692553f2a63" />


A lightweight, serverless, and secure P2P (Peer-to-Peer) file transfer web application built with WebRTC (via PeerJS). Share files instantly between any devices across the internet without any intermediary server storage.

## Features

- **Serverless & Privacy-First:** Files do not pass through a cloud server; they flow directly from device to device via end-to-end P2P connection.
- **Cross-Network Support:** Works not only on the same local Wi-Fi but also across different networks globally.
- **Zero Configuration:** Hosted entirely on static hosting platforms like GitHub Pages. No backend setup required.

## How It Works

1. Open the web app on both devices (e.g., your PC and your phone).
2. The app automatically generates a unique connection ID (`cs_xxxxxx`).
3. Enter the target device's ID into the connection panel and establish the secure tunnel.
4. Select any file to instantly stream it directly to the connected device.

## Tech Stack
- **Vanilla JavaScript** (FileReader & Blob API)
- **PeerJS (WebRTC Wrapper)** for signaling and P2P data channels

