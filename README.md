# API Documentation Style Guide

This style guide provides guidelines for Plaid Authorization Management API documentation and guides.

It includes s list of [words to avoid](#words-to-avoid)
an [internal word list](#internal-word-list),
[OpenAPI object rules](#openapi-object-rules),
and [miscellaneous tips](#miscellaneous-tips) to maintain consistency, where possible.

If something is not covered in this guide,
please default to the [Google style guide](https://developers.google.com/style).

[//]: # Alt: (&#40;please default to the [Microsoft style guide]&#40;https://docs.microsoft.com/en-us/style-guide/welcome/&#41;&#41;)

## Words to Avoid

Do not use these words unless you have a compelling reason.

- simply
- just
- easy
- easily
- should
- shouldn't

## Internal Word List

The following are common terms that often appear in the Capstone LLC docs.
Use the word or phrase as written and avoid variations where possible.

- **Partner**
  - Avoid
      - Plaid Partner
      - Plaid’s Data Access Partners
      - Institution
    - *Notes:*
      - Do not treat as a proper noun, (ex. don't capitalize, unless at the beginning of a sentence.)
      - Partners implement a Consent Portal which will list all the applications their users have given access to their data.
- **End User**
  - Avoid
    - User
  - *Notes:*
    - An end user is a person using our partner's app.
    - Do not treat as a proper noun, (ex. don't capitalize, unless at the beginning of a sentence.)
- **TK Scopes**

## OpenAPI Object Rules

Use the following rules to standardize formatting within the OpenAPI specification.

### Rules for Key-value Pairs
- Summaries:
  - Rules:
    - Title case
    - No period at the end
    - Infinitive verbs
  - Examples: 
    - YES: `"summary": "Get Auth Token"`
    - NO: `"summary": "Get Auth Token."`
    - NO: `"summary": "Get auth token."`
    - NO: `"summary": "Gets an Auth Token"`

- Descriptions:
  - Rules:
    - Present tense
    - Period at the end
  - Examples:
    - YES: `"description": "Returns an authentication token."`
    - NO: `"description": "Return an authentication token."`
    - NO: `"description": "Returns an authentication token"`

- Operation IDs:
  - Rules:
    - Concatenate all the words in the path, minus special characters
  - Example:
    ```
    "/sandbox/item/set_verification_status": {
      "operationId": "sandboxItemSetVerificationStatus"`
    }
    ```

### Other Rules
- Reuse a component if it appears three or more times.

## Miscellaneous Tips

Keep the following suggestions in mind, where possible, in order to maintain consistency.

- [Prefer English to Latin](https://developers.google.com/style/abbreviations?hl=en#dont-use)
    - Use 'for example' rather than 'e.g.', where possible.
- Never start a sentence with code
  - Examples:
    - YES: "The `user_id` is required."
    - NO: "`user_id` is required."
- Referencing endpoints in plain text:
  - Include the leading slash
      - Examples: 
        - YES: "Send a POST request to the `/payment/list.json` endpoint."
        - NO: "Send a request to `payment/list.json`."
- Capitalization:
  - Rules:
    - Capitalize proper nouns
    - Capitalize parameter names, endpoint names, or when referencing a specific object/entity.
    - Be wary of the temptation to over-capitalize. Nouns start to feel more proper when you're referring to them again and again.
  - Examples: 
    - YES: The Application allows you to...
    - YES: The Application ID is required.
    - YES: The Scopes object includes...
    - NO: You can use scopes to allow the user to...
    - NO: The Application allows you to...
- Use [semantic line breaks](https://sembr.org/).
- Period in list items:
  - Unordered lists: no period
  - Ordered lists: period


NOTES:
- user ID not User ID
