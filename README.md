# Capstone LLC API Documentation Style Guide

# Intro 
*This is a style guide for a fake organization: 'Capstone LLC'.
The general principles can be applied to most API documentation but should be adapted based on your use case and internal style preferences.
Be sure to compare this style guide with any current marketing style standards and merge, where necessary.*

This style guide provides guidelines for Capstone, LLC API documentation.

It includes s list of [words to avoid](#words-to-avoid)
an [internal word list](#internal-word-list),
[example objects](#example-objects),
and [miscellaneous tips](#miscellaneous-tips) to maintain consistency, where possible.

If something is not covered in this guide,
please default to the [Google style guide](https://developers.google.com/style).

[//]: # (&#40;please default to the [Microsoft style guide]&#40;https://docs.microsoft.com/en-us/style-guide/welcome/&#41;&#41;)

# Words to Avoid
Do not use these words unless you have a really good reason.

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

# Miscellaneous Tips

Keep the following suggestions in mind, where possible, in order to maintain consistency.

- [Prefer English to Latin](https://developers.google.com/style/abbreviations?hl=en#dont-use)
  - Use 'for example' rather than 'e.g.', where possible.
- Include the leading slash when referencing endpoints
  - Example: `/payment/list.json`
    - Not: `payment/list.json`
