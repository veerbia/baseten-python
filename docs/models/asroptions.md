# AsrOptions

Advanced settings for the ASR process.


## Fields

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `beam_size`                                                                | *Optional[int]*                                                            | :heavy_minus_sign:                                                         | Beam search size for decoding. Supported up to 5.                          |
| `length_penalty`                                                           | *Optional[float]*                                                          | :heavy_minus_sign:                                                         | Length penalty applied to ASR output. Only applicable when beam_size > 1.<br/> |