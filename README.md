# Heretic Android / Cloud Setup

A phone-friendly guide to launch [Heretic](https://github.com/p-e-w/heretic) from an Android browser using a hosted GPU notebook. The phone is the controller; model modification runs on a cloud GPU, not on the phone.

## Start

1. Open the [notebook in Google Colab](https://colab.research.google.com/github/Dragondry/heretic-android/blob/main/Heretic_Colab.ipynb).
2. Choose **Runtime → Change runtime type → GPU** and save.
3. Run notebook cells from top to bottom.
4. Choose a model that fits the GPU assigned to your session.
5. Save the output somewhere persistent before the runtime disconnects.

## Limitations

- This does **not** run Heretic on the Android phone. Heretic uses PyTorch and model-weight processing; a phone without suitable compute is not a realistic device for this task.
- Hosted GPU availability, memory, duration, and quotas vary. A free session is not guaranteed to fit every model.
- The example 4B model may exceed a particular runtime's memory. Select a smaller supported model if needed.
- Hosted runtime storage is temporary.
- Heretic modifies open-weight models; it does not modify ChatGPT or GPT-6.

## Privacy

Do not commit passwords, Hugging Face tokens, or private data to this public repository or notebook.

## Upstream

Use the official [Heretic source and README](https://github.com/p-e-w/heretic) for current requirements and configuration details.