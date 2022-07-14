---
description: >-
  Com esses usos de caracteres, você pode deixar o bot retornar os caracteres fornecidos
  sem aceitar isso como um separador ou como o fim de uma função.
---

# Escape de Caracteres

## Escape de Caracteres:

`[` => `#RIGHT#`

`]` => `#LEFT#`

`;` => `#SEMI#`

`:` => `#COLON#`

`$` => `#CHAR#`

`>` => `#RIGHT_CLICK#`

`<` => `#LEFT_CLICK#`

`=` => `#EQUAL#`

`}` => `#LEFT_BRACKET#`

`{` => `#RIGHT_BRACKET#`

## Mais:

Backspace => `\b`\
Form speed => `\f`\
New line =>\
Carriage Return =>\
Horizontal Tabulator =>\
Vertical Tabulator => `\v`\
Single quote => `\'`\
Double quote => `\"`\
Backslash => `\`

{% hint style="info" %}
Esses escapes de caracteres são úteis para usar caracteres especiais dentro de funções. Por exemplo, no campo de texto do [$sendMessage](../functions/usdsendmessage.md).
{% endhint %}
