# Audios
(*audios*)

## Overview

### Available Operations

* [transcribe](#transcribe) - Transcribe Audio

## transcribe

Use this endpoint to transcribe audio. Provide your audio input (as a URL, Base64-encoded string, or raw bytes) along with optional parameters to control transcription behavior.


### Example Usage

```python
from baseten import Baseten
import os

with Baseten(
    api_key_auth=os.getenv("BASETEN_API_KEY_AUTH", ""),
) as b_client:

    res = b_client.audios.transcribe(whisper_input={
        "audio": {
            "audio_b64": "<value>",
        },
    })

    # Handle response
    print(res)

```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `whisper_input`                                                     | [models.WhisperInput](../../models/whisperinput.md)                 | :heavy_check_mark:                                                  | Object containing audio and related parameters.                     |
| `retries`                                                           | [Optional[utils.RetryConfig]](../../models/utils/retryconfig.md)    | :heavy_minus_sign:                                                  | Configuration to override the default retry behavior of the client. |

### Response

**[models.TranscribeAudioResponse](../../models/transcribeaudioresponse.md)**

### Errors

| Error Type      | Status Code     | Content Type    |
| --------------- | --------------- | --------------- |
| models.APIError | 4XX, 5XX        | \*/\*           |