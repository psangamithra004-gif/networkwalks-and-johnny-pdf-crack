# networkwalks-and-johnny-pdf-crack
Password cracking lab using Networkwalks Hash Calculator &amp; John the Ripper (Johnny GUI) on Kali Linux. Includes hash extraction, wordlist attacks, and PDF password recovery.
# 🔐 Password Cracking Lab – Networkwalks Tools & John the Ripper (Kali Linux)

## 📌 Overview
This project demonstrates two different methods for recovering passwords from encrypted PDF files:
1. **Online Method:** Using the Networkwalks Hash Calculator and Password Cracker (browser-based).
2. **Local Method:** Using **John the Ripper (Jumbo)** and **Johnny** (GUI) on Kali Linux.

Both methods were performed in a **Kali Linux (VirtualBox)** environment.

## 🎯 Objective
- Download password-protected PDFs from the lab page.
- Extract a crackable hash using both online and local tools.
- Recover the PDF passwords to capture the flags.

## 🛠️ Tools Used
| Tool | Purpose |
|------|---------|
| Kali Linux 2026.1 (VM) | Operating System |
| Firefox ESR | Web Browser |
| Networkwalks Hash Calculator | Extract PDF hash (Online) |
| Networkwalks Password Cracker | Recover Password (Online) |
| **John the Ripper (Jumbo)** | **Local hash cracking engine** |
| **Johnny (GUI)** | **Graphical front-end for John** |
| `pdf2john` | Extract hash locally from PDF |

---

## 🧪 Method 1: Online (Networkwalks Tools)

### Step 1: Download the PDF
Downloaded `My-Locked-PDF1-1.pdf` from the lab page.

### Step 2: Extract the Hash
1. Opened the **Networkwalks Hash Calculator** (`https://networkwalks.com/hash-calculator/`).
2. Clicked the **PDF** tab.
3. Uploaded the locked PDF.
4. Copied the full hash starting from `$pdf$`.

### Step 3: Crack the Hash
1. Opened the **Networkwalks Password Cracker** (`https://networkwalks.com/password-cracker/`).
2. Pasted the hash and started the crack.
3. **Result:** Password recovered was `1qaz2wsx`.

---

## 🧪 Method 2: Local (John the Ripper + Johnny on Kali)

### Step 1: Install John the Ripper & Johnny
```bash
sudo apt update
sudo apt install john johnny
