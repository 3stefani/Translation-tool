# Example Case Study

## How to Test the Tool

Use this example to test the Translation Error Taxonomy & Annotation Tool.

---

## Test Case: Customer Service Email - Refund Request

### Project Details
- **Project Name**: Customer Service Email - Refund Request
- **Source Language**: English (US)
- **Target Language**: Spanish (Spain)
- **Content Type**: Customer service communication

---

### Source Text (English)
```
Dear customer,

We have processed your refund request. The amount will be credited to your account within 5-7 business days.

If you have any questions, please don't hesitate to contact us.

Best regards,
Customer Support Team
```

---

### Target Text (Spanish - with intentional errors for annotation)
```
Estimado cliente,

Hemos procesado su solicitud de reembolso. La cantidad será acreditada a su cuenta dentro de 5-7 días de negocio.

Si tienes cualquier pregunta, por favor no dudes en contactarnos.

Saludos,
Equipo de Soporte al Cliente
```

---

## Errors to Annotate

Here are the errors you should find and annotate:

### Error 1: "días de negocio"
- **Selected Text**: "días de negocio"
- **Category**: Accuracy
- **Type**: Mistranslation
- **Severity**: Major
- **Notes**: Direct translation from English "business days". In Spanish (Spain), the correct term is "días laborables" or "días hábiles"

### Error 2: "reembolso"
- **Selected Text**: "reembolso"
- **Category**: Terminology
- **Type**: Inappropriate Term
- **Severity**: Minor
- **Notes**: While technically correct, "devolución" is more commonly used in Spanish (Spain) for customer service contexts

### Error 3: "cantidad"
- **Selected Text**: "cantidad"
- **Category**: Terminology
- **Type**: Inappropriate Term
- **Severity**: Minor
- **Notes**: In financial contexts in Spain, "importe" is more appropriate than "cantidad"

### Error 4: "será acreditada"
- **Selected Text**: "será acreditada"
- **Category**: Style
- **Type**: Unidiomatic
- **Severity**: Minor
- **Notes**: Passive voice calque from English. More natural: "se abonará en su cuenta"

### Error 5: "tienes"
- **Selected Text**: "tienes"
- **Category**: Fluency
- **Type**: Inconsistency
- **Severity**: Major
- **Notes**: Inconsistent register. Started with formal "usted" (su) but switched to informal "tú" (tienes). Should be "tiene"

### Error 6: "Soporte al Cliente"
- **Selected Text**: "Soporte al Cliente"
- **Category**: Terminology
- **Type**: Inappropriate Term
- **Severity**: Minor
- **Notes**: In Spain, "Atención al Cliente" is the standard term, not "Soporte al Cliente"

### Error 7: "Saludos"
- **Selected Text**: "Saludos"
- **Category**: Style
- **Type**: Inappropriate Register
- **Severity**: Minor
- **Notes**: Too informal for this context. Better: "Reciba un cordial saludo" or "Atentamente"

---

## Expected Results

After annotating all 7 errors, you should see:

### Statistics
- **Total Errors**: 7
- **Critical**: 0
- **Major**: 2
- **Minor**: 5

### Error Distribution by Category
- Accuracy: 1
- Fluency: 1
- Style: 2
- Terminology: 3

---

## Corrected Version (Reference)

```
Estimado cliente:

Hemos tramitado su solicitud de devolución. El importe se abonará en su cuenta en un plazo de 5 a 7 días laborables.

Si tiene alguna pregunta, no dude en ponerse en contacto con nosotros.

Reciba un cordial saludo,
Equipo de Atención al Cliente
```

---

## Learning Points

This example demonstrates common issues in MT output:
1. **Lexical calques**: Direct word-for-word translations
2. **Register inconsistency**: Mixing formal and informal address
3. **Terminology choices**: Using less idiomatic terms
4. **Syntactic patterns**: Keeping source language structure

These are exactly the types of errors that MTPE professionals identify and correct daily!

---

## Try Your Own!

After testing with this example, try annotating your own translation pairs:
- Customer service emails
- Product descriptions
- Technical documentation
- Marketing content
- Social media posts

The tool helps you build a systematic approach to quality assessment!
