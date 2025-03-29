<!-- Start SDK Example Usage [usage] -->
```python
# Synchronous Example
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

</br>

The same SDK client can also be used to make asychronous requests by importing asyncio.
```python
# Asynchronous Example
import asyncio
from baseten import Baseten
import os

async def main():

    async with Baseten(
        api_key_auth=os.getenv("BASETEN_API_KEY_AUTH", ""),
    ) as b_client:

        res = await b_client.audios.transcribe_async(whisper_input={
            "audio": {
                "audio_b64": "<value>",
            },
        })

        # Handle response
        print(res)

asyncio.run(main())
```
<!-- End SDK Example Usage [usage] -->