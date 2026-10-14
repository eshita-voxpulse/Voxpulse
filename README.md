# VoxPulse - AI-Based Speech Quality Analyzer

VoxPulse ek advanced speech analysis prototype hai jise public speaking aur spoken delivery failures ko evaluate karne ke liye design kiya gaya hai. Yeh system subjective human opinions ko hatakar audio signal analytics ke zariye objective performance metrics aur easy actionable feedback provide karta hai.

## 🔗 Project Quick Links
* **Live Web Dashboard:** https://vercel.app
* **Demo Video (YouTube):** https://youtu.be *(Yahan apne daddy ke account wala YouTube link daal dena)*

## 🛠️ Software Architecture (Decoupled Design)
Hamare project ko ekdam lightweight aur scalable banane ke liye humne decoupled architecture use kiya hai:
* **Frontend (UI Layer):** Vanilla HTML5, CSS3, aur JavaScript framework jise instantaneous rendering ke liye Vercel par deploy kiya gaya hai.
* **Backend (Analytics Brain):** Standalone Python pipeline jo audio waveforms ko standard 16 kHz mono environment mein process karti hai.
* **Data Bridge:** Frontend aur backend aapas mein ek structured JSON payload (`evaluation_results.json`) ke zariye communication explore karte hain.

## 📊 Engineered Contrastive Dataset
Data quality over quantity ko prioritize karte huye, humne ElevenLabs stability parameters ke zariye ek hi shared rhetorical transcript par flaws ka gradient spectrum ready kiya hai:
* `speech_01_normal.mp3` - Standard baseline reference model.
* `speech_02_pause.mp3` - Monotone aur awkward structural silence breaks track.
* `speech_03_low_mumbling_volume.mp3` - Low energy whisper aur inaudible speech track.
* `speech_04_rushed.mp3` - Hyper-accelerated syntax distortion track.

## ⚙️ Core Technical Features
* **Advanced Feature Extraction:** Librosa library ke zariye Logarithmic Loudness Envelope (RMS dB) extraction aur pYIN algorithm se continuous F0 pitch tracking.
* **Temporal Grounding:** torchaudio MMS_FA CTC model se precise forced word alignment nikaalna aur Dynamic Time Warping (DTW) se exact millisecond deviation regions ko isolate karna.
* **Causal Feedback & AI Coach:** JSON parsed visual dashboard jo numerical errors ko color-coded Causal Explanation Cards aur ek interactive AI Chat Assistant box mein badalta hai.

## 👥 Team Matrix & Roles
* **Ishita (Lead Data Engineer):** Dataset sourcing, text transcription alignment, aur baseline generation.
* **Ananya (Senior Backend Developer):** Core Python audio feature processing aur mathematical framework mapping.
* **Anshika (Application UI Developer):** HTML/JS responsive web panel building, Vercel deployment, aur assistant integration.

