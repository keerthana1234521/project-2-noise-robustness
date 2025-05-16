🎙️ Speech Transcription and Homophone Detection with Wav2Vec2

This project processes an audio file using a pre-trained [Wav2Vec2](https://huggingface.co/facebook/wav2vec2-base-960h) model for automatic speech recognition (ASR), adds synthetic noise, transcribes the noisy audio, detects homophones, and visualizes the results with frequency plots and word clouds.

---

## 🧠 Features

- ✅ Load and preprocess audio files (`.wav`)
- 🎛️ Add synthetic Gaussian noise to audio
- 🧾 Transcribe speech using `facebook/wav2vec2-base-960h`
- 🔍 Detect common English homophones
- 📊 Visualize top word frequencies
- ☁️ Generate word clouds from transcriptions
- 📈 Show homophone distribution

---

## 🛠️ Dependencies

Install the following Python packages:

```bash
pip install torch torchaudio librosa soundfile matplotlib wordcloud transformers
📂 Project Structure
bash
Copy
Edit
.
├── main.py             # Main script
├── noisy_output.wav    # (Generated) Noisy version of input audio
├── hardvard.wav        # (Input) Audio file to process (change to your own)
└── README.md           # This file
🚀 How to Run
Place a .wav file (16kHz recommended) in your working directory.

Edit the path in main():

python
Copy
Edit
input_path = "/path/to/your/audio.wav"
Run the script:

bash
Copy
Edit
python main.py
🧠 Example Output
Transcription:

csharp
Copy
Edit
this is a sample transcription from the noisy audio
Homophones Detected:

vbnet
Copy
Edit
to → too, two
their → there, they're
Visualizations:

Top 10 most frequent words

Word cloud of all transcribed words

Bar chart of detected homophones

🧩 Extend Ideas
Use diarization or speaker segmentation

Apply to long audio via chunking

Build a GUI with Gradio or Streamlit

Evaluate accuracy using WER/CER metrics with jiwer

📄 License
MIT License © 2025
