# Web-P2P-Share ( u can use it right here) https://reveko0o.github.io/Web-p2p-share/

<img width="878" height="454" alt="image" src="https://github.com/user-attachments/assets/c3594191-dc16-4371-8886-2692553f2a63" />


A lightweight, serverless, and secure P2P (Peer-to-Peer) file transfer web application built with WebRTC (via PeerJS). Share files instantly between any devices across the internet without any intermediary server storage.

## Features

- **Serverless & Privacy-First:** Files do not pass through a cloud server; they flow directly from device to device via end-to-end P2P connection.
- **Cross-Network Support:** Works not only on the same local Wi-Fi but also across different networks globally.
- **Zero Configuration:** Hosted entirely on static hosting platforms like GitHub Pages. No backend setup required.

## How It Works

- **File Size Limit & Workflow:** 
  - **File Size Limit:** Since data is stored temporarily in the browser's memory (`ArrayBuffer` / `Blob`), extremely large files (e.g., 2-3 GB+) might hit browser RAM limits or cause crashes. However, it works flawlessly for a few megabytes of photos, documents, APKs, or small archives.
  - **Download Process:** When the sender selects a file, it is read into memory using `FileReader` and streamed securely as a data packet through the PeerJS data channel. On the receiver side, this data is automatically converted into a virtual file (`Blob`), triggering the browser's built-in download manager to save it directly to the device's "Downloads" folder.

1. Open the web app on both devices (e.g., your PC and your phone).
2. The app automatically generates a unique connection ID (`cs_xxxxxx`).
3. Enter the target device's ID into the connection panel and establish the secure tunnel.
4. Select any file to instantly stream it directly to the connected device.


