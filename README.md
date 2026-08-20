social media 
If you mean add an index.html entry point for your Happen app, here is a basic Flutter Web index.html:
HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">

  <meta name="viewport"
        content="width=device-width, initial-scale=1.0">

  <meta name="description"
        content="Happen - Connect, share and discover.">

  <title>Happen</title>

  <base href="/">

  <link rel="icon" type="image/png" href="favicon.png">

  <link rel="manifest" href="manifest.json">
</head>

<body>
  <script>
    // Flutter Web bootstrap
    {{flutter_bootstrap_js}}
  </script>
</body>
</html>
For a Flutter Happen project, this file normally goes at:
happen/
└── web/
    ├── index.html
    ├── manifest.json
    └── icons/
If your Happen project is Flutter Android-only, index.html isn't used for the Android APK; it's specifically the web entry point.
