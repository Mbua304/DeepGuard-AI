# DeepGuard AI 

A Multi-Modal Tool for Detecting AI-Generated Content (Text, Image, Audio, Video)

DeepGuard AI is a machine learning–powered detection tool that helps identify AI-generated content across multiple formats. It integrates pre-trained models for classification, feature extraction, and provides a clean Streamlit web interface for interactive use.

### Features

Multi-Modality Support

 Text (PDF, DOCX, TXT, RTF, ODT)

 Images (JPG, PNG, BMP, GIF, TIFF)

 Audio (WAV, MP3, FLAC, M4A, OGG, AAC)

 Video (MP4, MOV, AVI, MKV, WebM, WMV)

### Model Integration

prithivMLmods/Deep-Fake-Detector-v2-Model → Image detection

Gustking/wav2vec2-large-xlsr-deepfake-audio-classification → Audio detection

roberta-large-openai-detector → Text detection

Custom Thresholds

Adjustable confidence slider (e.g., 60%) for flexible verdicts.

Interactive UI

Built with Streamlit
 for a responsive, user-friendly interface.

### Results Dashboard

Displays AI-likelihood (%) with color-coded verdicts.

Detailed analysis view with model outputs.

## Tech Stack

Python 3.9+

Streamlit → Web UI

Transformers (Hugging Face) → ML Pipelines

PyTorch → Model backend

Librosa / SoundFile → Audio preprocessing

PIL (Pillow) → Image handling

PyMuPDF / python-docx / odfpy → Text extraction

### Installation

### Clone the repository:

git clone https://github.com/mbua304/deepguard-ai.git
cd deepguard-ai


### Create and activate a virtual environment (recommended):

python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows


Install dependencies:

pip install -r requirements.txt

 Usage

Run the Streamlit app:

streamlit run app.py


### Open the link in your browser (default: http://localhost:8501)

Select a modality (Text, Image, Audio, Video)

Upload your file or paste text directly

Click Analyze

View AI-likelihood results and details

 Project Structure
deepguard-ai/
├── app.py                # Main Streamlit app
├── utils.py              # Core analysis functions
├── requirements.txt      # Python dependencies
├── README.md             # Project documentation
└── ...

 Example Results

### Text: AI likelihood → 87.3%

### Audio: Correctly identifies bonafide speech

### Image: Flags synthetic image artifacts

 Acknowledgments

Models from Hugging Face Hub

Libraries: Streamlit, PyTorch, Librosa, PyMuPDF, ODFPy

## Acknowledgments
BNS Cyberlab LTD for the internship opportunity and guidance

Hugging Face for providing the pre-trained models

Streamlit for the excellent web application framework

The open-source community for various libraries and tools used

### Contact
Nelson Mosisah - @my linkedin - bmosisah20@gmail.com

Project Link: https://github.com/mbua304/deepguard-ai


### Disclaimer

This tool is intended for educational and research purposes only.
Results may vary depending on dataset quality, modality, and evolving AI models.
