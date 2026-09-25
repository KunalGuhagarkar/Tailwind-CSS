# Introduction and Tailwind Setup

[Tailwind Setup Link](https://tailwindcss.com/docs/installation/tailwind-cli)

## Tailwind CLI

Commands:

Install Tailwind via npm
``` bash
npm install tailwindcss @tailwindcss/cli
```

Import Tailwind in your CSS
``` css
@import "tailwindcss";
```

Start the Tailwind CLI build process
``` bash
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
```

Start using Tailwind in your HTML
``` html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```

## Lesson 1

index.html
``` html
<!doctype html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Tailwind Chapter 1</title>
        <link rel="stylesheet" href="./output.css" />
    </head>
    <body class="min-h-screen grid place-content-center radial-blue">
        <div
            class="bg-emerald-500 w-52 h-52 rounded-full shadow-2xl grid place-content-center"
        >
            <div
                class="bg-teal-200 w-32 h-32 rounded-full grid place-content-center"
            >
                <div class="bg-red-500 w-16 h-16 rounded-full"></div>
            </div>
        </div>
    </body>
</html>
```

style.css
``` css
@import "tailwindcss";

.radial-blue {
    background: radial-gradient(lightyellow, skyblue);
}
```

Output
![Output](image.png)