# Speech to Text Translator using WhisperX

This repository contains a Python-based **Speech-to-Text Translator** that uses the WhisperX model for audio transcription. The script processes `.mp3` and `.wav` audio files, transcribes them to text, and performs post-processing to clean and format the transcribed text.

## Features

- **Audio Processing**: Supports `.mp3` and `.wav` audio file formats.
- **Duration Check**: Automatically rejects audio files longer than 40 seconds.
- **Custom Digit Mapping**: Converts spelled-out digits (e.g., "three") to their numeric forms ("3").
- **Text Cleaning**:
  - Removes unnecessary spaces between digits.
  - Convert alphanumeric use cases into a unified format.
- **Custom Exception Handling**: Detects unsupported file formats and excessively long audio files.

## Pre-requisites

Before running the code, ensure you have the following installed:

- Python 3.10 or above
- Google Colab (or a local Python environment)
- The following Python libraries:
  - `whisperx`
  - `pydub`
  - `soundfile`

## Usage

- Place your audio file (.mp3 or .wav) in a directory accessible to the script.
- Update the file_path variable in the script with the path to your audio file.

## Limitations

- The script rejects audio files longer than 40 seconds.
- Language is defaulted to English (en) for transcription.
- Requires a stable internet connection for WhisperX model initialization and processing.

## Contributions
Always feel welcome to contribute! If you have suggestions for improving this project or want to report a bug, feel free to open an issue or submit a pull request.

## Future Enhancements

- Add support for other languages.
- Improve error handling for specific edge cases.
- Integrate speaker wise detection and transcription.

