# Assignment 6.1 — Box Model Inspection

## File 1: `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Model Inspection</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <h1>CSS Box Model Inspection</h1>

    <div class="box content-box">
        <h2>Content Box</h2>
        <p>This box uses content-box. Padding and border are added to the content width.</p>
    </div>

    <div class="box border-box">
        <h2>Border Box</h2>
        <p>This box uses border-box. Padding and border are included in the total width.</p>
    </div>

    <div class="box custom-box">
        <h2>Custom Box</h2>
        <p>This box uses different padding, border, and margin values.</p>
    </div>

</body>
</html>
```

## File 2: `style.css`

```css
body {
    font-family: Arial, sans-serif;
    background-color: #f1f5f9;
    color: #1e293b;
    padding: 20px;
}

h1 {
    text-align: center;
    color: #1d4ed8;
}

.box {
    width: 300px;
    background-color: white;
}

.content-box {
    box-sizing: content-box;
    padding: 20px;
    border: 5px solid blue;
    margin: 20px;
}

.border-box {
    box-sizing: border-box;
    padding: 20px;
    border: 5px solid green;
    margin: 30px;
}

.custom-box {
    box-sizing: content-box;
    padding: 30px;
    border: 8px solid orange;
    margin: 40px;
}
```

## Box Model Explanation

The CSS box model consists of four parts: content, padding, border, and margin. Content is the area where text appears. Padding is the space between the content and the border. Border surrounds the content and padding. Margin is the space outside the border.

## Difference Between Content-Box and Border-Box

The `content-box` model adds padding and border to the specified width. The `border-box` model includes padding and border within the specified width.

## Observation

Three boxes were created with different padding, border, and margin values. Chrome DevTools can be used to inspect the box model of each element.

## Box Model Labels

Content → Padding → Border → Margin