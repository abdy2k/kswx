# Khmer Word processor (`kswx`) 🇰🇭🦀

# Khmer Smart Writer (`kswx`) 🇰🇭🦀

A modern, memory-safe, and portable cross-platform word processor for the Khmer language, rewritten from the ground up in Rust. 

`kswx` is the official modern port of the historic **Khmer Smart Writer**, originally written in C++ for Windows 3.1 and Windows 95, developed by **Cambodian Software Development - Abdolgony Computer Services** and first released in 1992. This modern incarnation brings absolute crash resilience, modern text rendering, and native file compatibility to contemporary operating systems.

---

## ✨ Features

* **Legacy Heritage, Modern Core:** Upgraded from 1992 Windows 3.1 C++ code into a portable, blazing-fast Rust architecture.
* **Modern Khmer Engine:** Full native processing of Khmer text using clean UTF-8 code points within standard ranges:
  * `U+1780` to `U+17FF` (Khmer primary block)
  * `U+19E0` to `U+19FF` (Khmer Symbols block)
  * *Note: 99% of the Khmer Unicode set is supported. Obsolete/deprecated legacy code points are stripped or blocked to maintain strict modern compliance.*
* **Zero-Loss Crash Protection:** Built-in system failure file rescue. If your operating system crashes or loses power, simply reboot and restart Khmer Smart Writer. Your un-saved file is instantly located, and the app prompts you with options on how to recover your work.
* **Rich Document Layouts:**
  * **Advanced Tables:** Dynamic row generation via the upper `Insert` menu (Requires valid numeric inputs).
  * **Image Insertion:** Support for `.png`, `.jpg`, and `.jpeg` pictures with interactive scaling and resizing.
* **Typing Layout Integrity:** When operating in *Khmer Mode*, standard keyboard shortcuts are deactivated to prevent layout collisions and ensure seamless character cluster combination behavior.
* **Cross-Platform Compatibility:** Native document compilation and local hardware printing on both **Windows** and **Linux** distributions.

---

## 💾 Supported File Formats

`kswx` acts as a universal bridge between legacy systems and modern office standard formats. You can open and export files to:
* `.ksw` (Native Khmer Smart Writer Document format)
* `.docx` (Microsoft Word Document standard)
* `.odt` (OpenDocument Text standard)
* `.pdf` (Portable Document Format)

---

## 🛠️ User Guide

### Working with Tables
1. Navigate to the **Calc Spreadsheet...** menu at the top toolbar.
2. Navigate to the **Create...** menu at the top toolbar.
5. Navigate to the **Insert** menu at the top toolbar.
5. Select **Insert Row**.
5. *Constraint:* Please verify that any dimensions or row counts typed into the prompt box are **valid numbers** to prevent execution errors.

### Handling Images
1. Use the image attachment dialog to import images (`.png`, `.jpg`, or `.jpeg`).
2. Click and drag the corner boundaries of the placed graphic to resize it dynamically to fit your column widths.

### Understanding Khmer Mode Typing
To ensure that character stacking, subscript vowels, and diacritics map exactly to your keys without triggering unintended system behaviors, **system/application keyboard shortcuts are completely disabled when Khmer input mode is active**. Switch back to default Latin input mode to resume standard interface hotkeys.
You may display on screen static keyboard layour to help you locate Khmer letter and key combination.

### Understanding Tools 
1. Language checked for Khmer/English
2. Khmer
3. English
4. Keyboard Layout (OnScreen Keyboard On/Off) 
---
<img width="748" height="510" alt="image" src="https://github.com/user-attachments/assets/45a66cc6-5409-4b90-be8f-c2fec588e0df" />


## 🧪 Beta Testing Status

`kswx` is currently under active beta testing. We are verifying core layout stability, print rendering across Linux CUPS and Windows spoolers, and the recovery prompt cycle during accidental power losses.

Please report any incorrect rendering behavior or edge cases involving the text engine boundary layers to our project repository issue tracker.
