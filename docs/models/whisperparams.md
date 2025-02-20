# WhisperParams

Parameters for controlling Whisper’s behavior.


## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `prompt`                                                                            | *Optional[str]*                                                                     | :heavy_minus_sign:                                                                  | Optional transcription prompt.                                                      |
| `audio_language`                                                                    | *Optional[str]*                                                                     | :heavy_minus_sign:                                                                  | Language of the input audio. Set to "auto" for automatic detection.<br/>            |
| `language_detection_only`                                                           | *Optional[bool]*                                                                    | :heavy_minus_sign:                                                                  | If true, only return the automatic language detection result without transcribing.<br/> |
| `use_dynamic_preprocessing`                                                         | *Optional[bool]*                                                                    | :heavy_minus_sign:                                                                  | Enables dynamic range compression to process audio with variable loudness.<br/>     |