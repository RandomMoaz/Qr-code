# 🚀 QR Code Generator

A simple and efficient QR code generator built with Python. This project allows you to create QR codes from text or URLs and customize their appearance.

## ✨ Features
- ✅ Generate QR codes from text or URLs
- 🎨 Customize QR code color and background
- 💾 Save QR codes as image files

## 📦 Requirements
Make sure you have the following installed before running the script:

```sh
pip install qrcode[pil]
```

## ⚙️ Installation & Usage
1. 📥 Clone the repository:
   ```sh
   git clone https://github.com/RandomMoaz/Qr-code.git
   cd Qr-code
   ```
2. 📦 Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. ▶️ Run the script:
   ```sh
   python Qr_code_generator.py
   ```

## 🔍 Example
Modify the script to generate a QR code for any text or URL:

```python
import qrcode

qr = qrcode.QRCode(
    version=1,
    error_correction=qrcode.constants.ERROR_CORRECT_L,
    box_size=10,
    border=4,
)
qr.add_data("https://example.com")
qr.make(fit=True)

image = qr.make_image(fill_color="black", back_color="white")
image.show()
image.save("qrcode.png")
```

## 🛠️ Troubleshooting
If you encounter `ModuleNotFoundError: No module named 'PIL'`, install Pillow:
```sh
pip install Pillow
```

## 🤝 Contributing
Feel free to fork this repository, make improvements, and submit pull requests!


## 📜 License
This project is licensed under the MIT License.
