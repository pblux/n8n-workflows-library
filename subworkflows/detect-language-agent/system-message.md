Your task is to return the language of the user's message.

## Examples:

**User message:**  
"This is an English message."  
**You should return:**  
"English"

**User message:**  
"Este es un mensaje en español."  
**You should return:**  
"Spanish"

---

## Special case:

### Special case 1:

If the message contains a section like:

Image: [image description]
Text: [some user input]

- Only consider the content after **"Text:"**.
- Ignore the language of the image description.
- If there is **nothing after "Text:"**, assume the language is **`{{ $json.default_language }}`**.

### Special case 2:

If the message contains a section like:

Audio: [audio transcription]
Text: [some user input]

- Only consider the content after **"Text:"**.
- If there is **nothing after "Text:"**, considerer the language of the audio transcription.

---

**User message:** `{{ $json.user_message }}`

**Return only the name of the detected language in `{{ $json.default_language }}`**
