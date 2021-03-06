Prefixes
========

We add prefixes to splynx for identify the calls when the CDR is imported. We could also import all prefixes from a .csv file.

In Voice → Prefixes, click on add.

![Add prefixes](./add_prefixes.png?w=300)

Complete the fields.

![Create prefixes](./create_prefixes.png?w=300)

* **Prefix** - Add the prefix using the following patterns

You can use phone patterns for match phone numbers group.
Patterns are created with using special symbols.
Example pattern for Angola phone numbers: `244{.}`.

---

#### Special symbols:

| Symbol      | Description                                                                       |
|-------------|-----------------------------------------------------------------------------------|
| `{x}`       | One digit from 0 to 9.                                                            |
| `{z}`       | One digit from 1 to 9.                                                            |
| `{n}`       | One digit from 2 to 9.                                                            |
| `{!}`       | Zero or more any characters.                                                      |
| `{.}`       | One or more any characters.                                                       |
| `{100-300}` | Number between 100 and 300. You can use any numbers instead of 100 and 300.       |
| `{123|456}` | One of "123" or "456". You can use any string pattern instead of "123" and "456". |

---

#### Examples:

| Phone pattern        | Description                                                                             |
|----------------------|-----------------------------------------------------------------------------------------|
| `+28050420{30-40}`   | Phone must begin with "+28050420" and end with number from 30 to 40.                    |
| `{380|250}{x}{x}{x}` | Phone must begin with one of "380" or "250". Then must be three digit from 0 to 9       |
| `{z}{3|4}{n}{n}`     | Phone must begin with digit from 1 to 9. Then "3" or "4" and then two digit from 2 to 9 |
| `{!}`                | Any phone number                                                                        |


* **Destination** - Field for identify which type of destination is that prefix, like international, fixed, mobile...etc.


* **Rate Type** - Set Call, SMS or Data.


* **Category ID** - Select the category. Should be previously added.


Other way is to use the import tool.
![Import tool](./import.png?w=300)