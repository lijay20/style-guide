# API Documentation Style Guide

This style guide provides guidelines for Capstone, LLC API documentation.

It includes a list of [words to avoid](#words-to-avoid)
an [internal word list](#internal-word-list),
[example objects](#example-objects),
and [miscellaneous tips](#miscellaneous-tips) to maintain consistency, where possible.

If something is not covered in this guide,
please default to the [Google style guide](https://developers.google.com/style).

[//]: # (&#40;please default to the [Microsoft style guide]&#40;https://docs.microsoft.com/en-us/style-guide/welcome/&#41;&#41;)

# Words to Avoid
Do not use these words unless you have a compelling reason.

- simply
- just
- easy
- easily
- should
- shouldn't
- Kulas PLC (We white-label their products, so avoid this company name in the docs!)

# Internal Word List

The following are common terms that often appear in the Capstone LLC docs.
Use the word or phrase as written and avoid variations where possible.

- **Capstone**
  - Avoid
    - Cap Stone
    - Cap stone
    - CapStone
- **E-ticket**
  - Avoid
    - eticket
    - eTicket
  - Capitalize as normal in sentences and titles.
    - Example 1: "Add the e-ticket to your order."
      - Not: "Add the E-ticket to your order."
    - Example 2 (Title): "How to Add an E-ticket"
      - Not: "How to Add an E-Ticket"
- **E-commerce**
  - Avoid
    - ecommerce
    - eCommerce
  - (Same capitalization rules as 'e-ticket', above.)
- **JSON**
  - Avoid: 
    - json
    - .json
    - Json
  - *Note:* Watch out for auto-correct trying to swap this out for Jason. 

# Common Phrases
Below is a list of common phrases that appear often in the API reference docs.
Use the phrase as closely as possible.

- "Refer to the `/v3/payment.json` endpoint."
  - Avoid: "Refer to 'payment'."

# Example Objects

The following example objects can be used as needed.

## Salesperson
- Name: Anjelica Taylor
  - User ID: 388420
  - Hired Date: '2022-11-02'
  - Category: I9

## Payment Object
- Cardholder Name: Wes Hroch
  - CC number: 4263982640269299
  - Exp date: 02/2023
  - CVV: 940
  - Amount: $298.00

# OpenAPI Spec
## HTTP Methods
When referencing HTTP methods, use all caps, never lowercase.
- GET
- PUT
- POST
- PATCH
- DELETE

## Keys
### Descriptions
- Descriptions for parameters, schemas and object descriptions should end in a period.
  - Example: `"description": "Returns an payment object."`
- Use present tense
  - Example: "Returns a payment object."
    - Not: "Return a payment object."
- The description come *first*, followed by any modifiers
  - Example: `"description": "The payment ID. (Read-only)"`
    - Not: `"description": "Read-only. The payment ID."`

### Summaries
- Use title case
- No period at the end
- (Summaries generally appear as the title of the endpoint in most tools.)

### Operation IDs
- Use [camelCase](https://en.wikipedia.org/wiki/Camel_case)
  - Example: `"operationId": "getPaymentObject"`

# Miscellaneous Tips

Keep the following suggestions in mind, where possible, in order to maintain consistency.

- [Prefer English to Latin](https://developers.google.com/style/abbreviations?hl=en#dont-use)
  - Use 'for example' rather than 'e.g.', where possible.
- Include the leading slash when referencing endpoints
  - Example: `/payment/list.json`
    - Not: `payment/list.json`
- - Never start a sentence with code
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
