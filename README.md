# Versa RES - Floor Plan Extractor

Welcome to the **Floor Plan Extractor**, a powerful desktop application built to streamline the real estate marketing process. This tool allows you to instantly extract clean, professional floor plans from complex architectural PDFs and customize them with your own branding, all using advanced AI and Computer Vision.

## 🚀 Features

- **Automated Floor Plan Extraction:** Upload raw, messy architectural PDFs and let the app intelligently extract just the floor plan lines, making the background completely transparent.
- **Advanced AI Noise Scrubbing:** Powered by Google's Gemini Vision API (Nano Banana Pro), the app automatically detects and erases structural noise, measurements, and architectural clutter that shouldn't be in a consumer-facing marketing plan.
- **Smart Deskew & Perspective Correction:** Easily correct slanted or photographed floor plans using a 4-point perspective crop tool.
- **Custom Branding & Templates:** Add your own logos, watermarks, text, and custom background templates. Create a signature look for your properties.
- **Cloud Synchronization:** Log in with your license key on any computer, and the app will automatically sync your custom templates and metadata from the cloud, ensuring your workspace is always exactly how you left it.
- **Offline & Local-First:** All high-resolution image processing and compositing is done securely on your local machine using a bundled Python backend, ensuring maximum privacy for your client documents.

## 📥 Download & Installation

You can download the latest version of the Floor Plan Extractor for your operating system from the [Releases page](../../releases/latest).

### Available Platforms:
- **macOS** (`.dmg` file - Apple Silicon and Intel supported)
- **Windows** (`.exe` installer)

### Getting Started:
1. Download the installer for your OS.
2. Run the installer and open the app.
3. Enter your active **License Key** to authenticate your device.
4. Upload your first PDF and start extracting!

## 🔐 Licensing

This application requires an active license key to operate. 
If you do not have a license key, you can purchase one through the [Floor Plan Extractor Web Portal](https://floorplan.artistsarescientists.com/).

License keys are tied to your email address and can be used to activate the app on up to 5 concurrent devices. Your custom templates are synced automatically across all activated devices.

## 🛠️ Technical Architecture

While this repository hosts the compiled releases, the underlying architecture consists of two proprietary, closed-source codebases:

1. **The Desktop App:** Built with Electron, HTML/JS for the frontend, and a bundled FastAPI Python backend. It utilizes OpenCV and PyMuPDF for heavy image manipulation and SAM (Segment Anything Model) logic.
2. **The Cloud Backend:** A serverless Google Cloud Run application that handles license generation (Stripe), Google/Microsoft OAuth, Cloud Syncing, and AI orchestration (Gemini API).

## 💬 Support & Feedback

If you encounter any bugs, crashes, or feature requests, please submit an issue on the [Issues tab](../../issues) of this repository. Be sure to include your operating system and the version of the app you are running.

---
*Built by James Zayner and the Versa RES Team.*
