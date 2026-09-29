# KotoType third-party notices

KotoType includes code derived from Handy by CJ Pais (2025), licensed under
the MIT License. The license text is included as `LICENSE` in this directory.

The bundled local polishing server is llama.cpp, revision `b11174`, by the
llama.cpp contributors, licensed under the MIT License. Its license text is
included as `LLAMA_CPP_LICENSE` in this directory. Source:
<https://github.com/ggml-org/llama.cpp/tree/b11174>.

The bundled `libomp.dll` from the llama.cpp Windows package is LLVM OpenMP,
licensed under Apache License 2.0 with LLVM Exceptions. The complete text from
the same pinned package is included as `LICENSE-LLVM-OpenMP`.

The bundled speech-recognition runtime (`transcribe.dll` and its ggml DLLs)
comes from `transcribe-cpp` 0.2.3 and `transcribe-cpp-sys` 0.2.3, including
ggml and miniz. Their license texts are included as
`TRANSCRIBE_CPP_LICENSE`, `GGML_LICENSE`, and `MINIZ_LICENSE`.
Source: <https://github.com/handy-computer/transcribe.cpp>.

The bundled `silero_vad_v4.onnx` voice activity model is from Silero VAD
under the MIT License. Its text is included as `SILERO_VAD_LICENSE`.
Source: <https://github.com/snakers4/silero-vad>.

ONNX Runtime is used for ONNX model execution under the MIT License. Its
license text is included as `ONNX_RUNTIME_LICENSE`.
Source: <https://github.com/microsoft/onnxruntime>.

The standard speech-recognition model is
`handy-computer/whisper-large-v3-turbo-gguf`, distributed separately under
Apache License 2.0:
<https://huggingface.co/handy-computer/whisper-large-v3-turbo-gguf>.

The optional four-part local polishing model is a split copy of
`unsloth/gemma-4-12b-it-GGUF` (`gemma-4-12b-it-Q4_K_M.gguf`), a quantization
of `google/gemma-4-12b-it`. The source repository declares Apache License
2.0. Model sources:
<https://huggingface.co/unsloth/gemma-4-12b-it-GGUF> and
<https://huggingface.co/google/gemma-4-12b-it>.

These models are downloaded separately from the installer. Their attribution
and license also appear on the download page. The Apache License 2.0 text is
included as `APACHE-2.0.txt` in this directory.
