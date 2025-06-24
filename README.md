# 📚 XML Bookstore with DTD and XSD Validation

## ✅ Objective

To create an XML representation of a bookstore and validate it using both:

- **DTD (Document Type Definition)**
- **XSD (XML Schema Definition)**

---

## 📁 Files Included

### `bookstore.xml`
Contains the data structure for a bookstore with a list of books, including:

- Title (with language attribute)
- Author
- Year
- Price
- Category attribute for each book

### `bookstore.dtd`
Defines the allowed structure and elements for validation using DTD:

- Element hierarchy
- Attributes required for `book` and `title`

### `bookstore.xsd`
Defines a schema using XML Schema Definition (XSD) with:

- Strong typing (`xs:string`, `xs:decimal`, `xs:short`)
- Required attributes
- Support for multiple `<book>` entries

---

## 🧪 Validation

### DTD:
- Linked using `<!DOCTYPE bookstore SYSTEM "bookstore.dtd">`
- Validated using [xmlvalidation.com](https://www.xmlvalidation.com/) or browser

### XSD:
- Linked using:
  ```xml
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:noNamespaceSchemaLocation="bookstore.xsd"
