# TranscribeAudioResponseBody

Successful transcription response.


## Fields

| Field                                          | Type                                           | Required                                       | Description                                    |
| ---------------------------------------------- | ---------------------------------------------- | ---------------------------------------------- | ---------------------------------------------- |
| `language_code`                                | *Optional[str]*                                | :heavy_minus_sign:                             | Detected language code.                        |
| `language_prob`                                | *OptionalNullable[float]*                      | :heavy_minus_sign:                             | Confidence score for language detection.       |
| `segments`                                     | List[[models.Segments](../models/segments.md)] | :heavy_minus_sign:                             | List of transcribed segments.                  |