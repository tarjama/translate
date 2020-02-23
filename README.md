# Overview
Machine Translation (MT) service is a form of automated translation where the computer translates text without human involvement. Our enterprise clients use it to increase their productivity, save time, and decrease costs, as the MT is capable of translating entire documents in seconds. All texts and documents are kept 100% confidential within the tool, ensuring our clients the security and confidentiality they require for their sensitive documents and information.

## Encoding of the input text

The text should be in UTF-8 only.


## Code Sample

The following is showing an example using `POST` method.
```

curl -X POST 'https://mt.cleverso.com/mt/translate/sentence/' \
-F 'client=<CLIENT_ID>' \
-F 'access_token=<YOUR_TOKEN_ID>' \
-F 'inputText=<TEXT_SAMPLE_FOR_TRANSLATION>' 
```

The successful response will be:

```diff
HTTP 200 OK
Allow: POST, OPTIONS
Content-Type: application/json
Vary: Accept

{
    "translatedText": "الترجمة باللغة العربية",
    "originalText": "<TEXT_SAMPLE_FOR_TRANSLATION>"
}
```


